<h1>Pocket Fox</h1>
A portable cybersecurity research and penetration testing platform designed for security professionals, researchers, and enthusiasts.

<h2>Overview</h2>
Pocket-Fox is an all-in-one handheld cybersecurity research device designed to combine the capabilities of multiple security devices into a single expandable unit.

Pocket-Fox was lightly inspired by the following devices:
<ul>
  <li>Flipper Zero</li>
  <li>HackRF One</li>
  <li>WiFi Pineapple</li>
  <li>ESP32 Marauder</li>
  <li>Cyberdeck</li>
  <li>Pwnagotchi</li>
</ul>
It's aimed to bring some of the largest pentesting tools into a single unit, down to about 6x8x1.5".

<h2>The Goal</h2>
Pocket-Fox is being designed to provide:
<ul>
  <li>A portable cybersecurity research platform</li>
  <li>Modular hardware expansion</li>
  <li>Embedded security experimentation</li>
  <li>Wireless research capabilities</li>
  <li>Customizable software</li>
</ul>

<h2>Intended Users</h2>
Pocket-Fox is intended for:
<ul>
  <li>Cybersecurity students</li>
  <li>Security researchers</li>
  <li>Pentesters</li>
  <li>Hardware enthusiasts</li>
  <li>Makers</li>
</ul>

<h2>Hardware Concept</h2>

The current hardware concept is built around the <strong>Orange Pi Zero 3 (4GB)</strong> as the
main controller, with <strong>dual ESP32-S3-Super-Mini</strong> boards handling dedicated radio
subsystems.

<h3>Main Controllers</h3>
<ul>
  <li><strong>Orange Pi Zero 3 (4GB)</strong> — primary compute, UI, storage, and orchestration. Runs Linux-based tooling (e.g. bettercap, pwnagotchi-style agents) and drives the main screen.</li>
  <li><strong>2x ESP32-S3-Super-Mini</strong> — dedicated radio controllers, offloading time-sensitive or low-level radio work from the Orange Pi:
    <ul>
      <li>One handles sub-GHz, NFC, RFID, and IR peripherals.</li>
      <li>One is dedicated to onboard 802.11 WiFi work — monitor mode, packet sniffing, and deauth (native ESP32-S3 capability), reporting results back to the Orange Pi over serial.</li>
    </ul>
  </li>
</ul>

<h3>RF Subsystems</h3>
<ul>
  <li><strong>CC1101</strong> — sub-GHz transceiver (315/433/868/915MHz) for key fobs, garage doors, and other sub-GHz signals.</li>
  <li><strong>NRF24L01+PA+LNA</strong> — fixed 2.4GHz proprietary radio (not WiFi/802.11). Used for HID/mouse-jacking-style attacks against wireless mice and keyboards that use NRF24-based USB dongles.</li>
  <li><strong>ESP32-S3 onboard WiFi</strong> — 802.11 b/g/n, 2.4GHz only. Handles monitor mode, packet capture, and deauth/injection duties (Marauder-style), since neither the CC1101 nor the NRF24L01 can perform these functions.</li>
</ul>

<h3>NFC / RFID</h3>
<ul>
  <li><strong>PN532</strong> — 13.56MHz NFC reader/writer with antenna.</li>
  <li><strong>RDM6300</strong> — 125kHz RFID reader module.</li>
</ul>

<h3>IR</h3>
IR LED (TX) + TSOP-series IR receiver (RX) for universal remote / IR replay functionality.

<h3>Display</h3>
<strong>Waveshare 3.5" resistive TFT</strong> — exact interface (SPI / DPI-parallel / HDMI) TBD; interface choice affects Orange Pi driver complexity and should be confirmed against the specific Waveshare model before finalizing.

<h3>Power</h3>
<ul>
  <li><strong>7500mAh single-cell LiPo battery</strong></li>
  <li><strong>TP4056</strong> charging module (single-cell LiPo charge management)</li>
  <li><strong>Buck-boost converter</strong> (e.g. TPS63020-based) to provide a stable 5V rail to the Orange Pi regardless of battery charge state (3.0-4.2V range)</li>
  <li><strong>3.3V buck/LDO</strong> off the 5V rail to power the ESP32-S3 boards and radio modules (CC1101, PN532, RDM6300, NRF24L01)</li>
</ul>

<h3>Enclosure</h3>
Single 3D-printed case housing all subsystems, target dimensions 6" x 8" x 1.5-2".

<h3>Known Open Items</h3>
<ul>
  <li>Confirm exact Waveshare display model/interface</li>
  <li>Confirm final buck-boost converter part</li>
  <li>WiFi monitor-mode/injection currently scoped to ESP32-S3 onboard radio (2.4GHz only); external monitor-mode USB adapter (e.g. MT7612U-based) is a possible future addition for 5GHz / Orange-Pi-side capture, but not required for v1</li>
</ul>

<h2>Design Philosophy</h2>
Pocket-Fox is built around three principles:

<h3>Portability</h3>
<p>A complete security research environment which can be carried anywhere.</p>

<h3>Expandability</h3>
<p>Designed with modular hardware and software so new capabilities can be added over time.</p>

<h3>Educational</h3>
<p>Focused on learning how hardware, software, and cybersecurity systems work together.</p>
