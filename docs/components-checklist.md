<h1>Components List</h1>
<p>Running bill of materials for Pocket-Fox. Update links/costs as parts are finalized.</p>

<h1>Main Computing</h1>
  <h2>Main Computer</h2>
    <p><a href="https://www.amazon.com/gp/product/B0C9ZZKNL4/ref=ewc_pr_img_13?smid=APISWSAHKR1AT">Orange Pi Zero 3 4Gb</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$40</li>
      <li>Purpose: Primary compute, UI, storage, orchestration. Runs Linux-based tooling and drives the main screen.</li>
    </ul>
  <h2>Secondary Computing</h2>
    <p><a href="https://www.amazon.com/AITRIP-Supermini-Development-Dual-Core-Arduino%EF%BC%883PCS/dp/B0FKSKR2VL/ref=sr_1_16?s=electronics&sr=1-16">ESP-32-S3-Supermini (3-pack)</a></p>
    <ul>
      <li>Qty: 2 used, 1 spare</li>
      <li>Cost: ~$20 (for 3-pack)</li>
      <li>Purpose: Dedicated radio controllers. One drives sub-GHz/NFC/RFID/IR peripherals; one handles onboard WiFi monitor mode/deauth.</li>
    </ul>

<h1>RF Subsystems</h1>
  <h2>Sub-GHz</h2>
    <p><a href="">CC1101 Sub-GHz Transceiver Breakout</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$4-6</li>
      <li>Purpose: 315/433/868/915MHz transmit/receive — key fobs, garage doors, sensors.</li>
    </ul>
  <h2>2.4GHz (HID/Mousejacking)</h2>
    <p><a href="">NRF24L01+PA+LNA</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$5-8</li>
      <li>Purpose: Fixed 2.4GHz proprietary radio. HID/mousejacking-style attacks against NRF24-based wireless mouse/keyboard dongles. Not WiFi/802.11.</li>
    </ul>

<h1>NFC / RFID</h1>
  <h2>NFC</h2>
    <p><a href="">PN532 NFC Module (with antenna)</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$6-9</li>
      <li>Purpose: 13.56MHz NFC read/write.</li>
    </ul>
  <h2>RFID</h2>
    <p><a href="">RDM6300 125kHz RFID Reader Module</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$3-5</li>
      <li>Purpose: 125kHz RFID (EM4100-type tags).</li>
    </ul>

<h1>IR</h1>
  <p><a href="">IR LED + TSOP IR Receiver</a></p>
  <ul>
    <li>Qty: 1 each</li>
    <li>Cost: ~$2-3</li>
    <li>Purpose: Universal remote transmit/capture and IR replay.</li>
  </ul>

<h1>Display</h1>
  <p><a href="">Waveshare 3.5" Resistive TFT — TBD (confirm interface: SPI / DPI / HDMI)</a></p>
  <ul>
    <li>Qty: 1</li>
    <li>Cost: ~$20-35 (varies by interface)</li>
    <li>Purpose: Main UI, driven by Orange Pi.</li>
    <li>Status: Open item — model/interface not finalized.</li>
  </ul>

<h1>Power</h1>
  <h2>Battery</h2>
    <p><a href="">7500mAh Single-Cell LiPo Battery</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$12-18</li>
    </ul>
  <h2>Charging</h2>
    <p><a href="">TP4056 Charging Module</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$1-2</li>
      <li>Purpose: Single-cell LiPo charge management.</li>
    </ul>
  <h2>Power Conversion</h2>
    <p><a href="">Buck-Boost Converter — TBD (e.g. TPS63020-based)</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$5-10</li>
      <li>Purpose: Stable 5V rail to Orange Pi across full 3.0-4.2V battery range.</li>
      <li>Status: Open item — part not finalized.</li>
    </ul>
    <p><a href="">3.3V Buck/LDO Converter</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$2-5</li>
      <li>Purpose: Powers ESP32-S3 boards and radio modules off the 5V rail.</li>
    </ul>

<h1>Enclosure / Misc</h1>
  <ul>
    <li>3D printed case (6" x 8" x 1.5-2") — filament cost, ~$10-20</li>
    <li>Perfboard/protoboard — ~$5</li>
    <li>Wiring, headers, connectors, switches — ~$15-20</li>
  </ul>
