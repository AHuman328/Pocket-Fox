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
    <p><a href="https://www.aliexpress.us/item/3256807251509676.html?spm=a2g0o.detail.pcDetailTopMoreOtherSeller.1.3d0cW3LzW3LzIT&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=59298119-03e6-4699-a15d-6def8ae70b15&_t=gps-id%3ApcDetailTopMoreOtherSeller%2Cscm-url%3A1007.40050.354490.0%2Cpvid%3A59298119-03e6-4699-a15d-6def8ae70b15%2Ctpp_buckets%3A668%232846%238113%231998&pdp_ext_f=%7B%22order%22%3A%22626%22%2C%22eval%22%3A%221%22%2C%22sceneId%22%3A%2230050%22%2C%22fromPage%22%3A%22recommend%22%7D&pdp_npi=6%40dis%21USD%212.50%210.99%21%21%212.50%210.99%21%4021030f8317836310937694291e1096%2112000042531917568%21rec%21US%217891393102%21ABX%211%210%21n_tag%3A-29910%3Bd%3A7f0086b2%3Bm03_new_user%3A-29895%3BpisId%3A5000000207262906&utparam-url=scene%3ApcDetailTopMoreOtherSeller%7Cquery_from%3A%7Cx_object_id%3A1005007437824428%7C_p_origin_prod%3A">CC1101 Sub-GHz Transceiver Breakout</a></p>
    <ul>
      <li>Qty: 1 pack of Short Antenna 5pc</li>
      <li>Cost: $14.66-16.66</li>
      <li>Purpose: 1 for 315/433 another for 868/915MHz transmit/receive — key fobs, garage doors, sensors.</li>
    </ul>
  <h2>2.4GHz NRF24L01 + PA + LNA</h2>
    <p><a href="https://kitsguru.com/products/nrf24l01-antenna-v5-0-pa-lna-sma-wireless-module-8-pin-1100-meters?variant=40708860412085">NRF24L01+PA+LNA</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $1.56</li>
      <li>Purpose: Fixed 2.4GHz proprietary radio. HID/mousejacking-style attacks against NRF24-based wireless mouse/keyboard dongles. Not WiFi/802.11.</li>
    </ul>
  <h2>DollaTek 868-915MHz Antenna</h2>
    <p><a href="https://amzn.eu/d/0ilglMZ5">DollaTek 868-915MHz Antenna</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $10.28</li>
      <li>Purpose: To be able to use 868-915 and 315-433 at the same time with two antennas</li>
    </ul>
    <h2>Kaunosta 315/433 combo</h2>
    <p><a href="https://a.co/d/05Yy9hbk">Kaunosta 315/433 combo</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $16.99</li>
      <li>Purpose: To be able to use 868-915 and 315-433 at the same time with two antennas</li>
    </ul>
    
<h1>NFC / RFID</h1>
  <h2>NFC</h2>
    <p><a href="https://a.co/d/04TOuQiZ">PN532 NFC Module (with antenna)</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $8.99</li>
      <li>Purpose: 13.56MHz NFC read/write.</li>
    </ul>
  <h2>RFID</h2>
    <p><a href="https://a.co/d/04jA2o2r">RDM6300 125kHz RFID Reader Module</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $6:14</li>
      <li>Purpose: 125kHz RFID (EM4100-type tags).</li>
    </ul>

<h1>IR</h1>
  <p><a href="https://a.co/d/09up93EG">10pcs Bundle: 5x TSOP38238 (IR Receiver) + 5x TSAL6200 (940nm High-Power IR LED)</a></p>
  <ul>
    <li>Qty: 1 each used (spares from bundle)</li>
    <li>Cost: $8.99</li>
    <li>RX: TSOP38238 — 38kHz demodulating IR receiver, 3-pin, direct to GPIO</li>
    <li>TX: TSAL6200 — 940nm high-power IR LED, 100mA continuous (1.5A surge), needs small transistor driver (e.g. 2N2222 + resistors, ~$0.15) since ESP32 GPIO can't source 100mA directly</li>
    <li>Purpose: Universal remote transmit/capture and IR replay.</li>
    <li>Status: Finalized.</li>
  </ul>

<h1>Display</h1>
  <p><a href="https://www.waveshare.com/4.3inch-hdmi-lcd-b.htm">Waveshare 4.3inch Capacitive Touch Screen LCD (B)</a></p>
  <ul>
    <li>Qty: 1</li>
    <li>Cost: ~$49.99</li>
    <li>Interface: HDMI (display) + USB (capacitive touch, HID-class — no custom driver needed)</li>
    <li>Resolution: 800x480, IPS panel, 5-point capacitive touch</li>
    <li>Purpose: Main UI, driven by Orange Pi. Needs micro-HDMI adapter/cable for Orange Pi Zero 3's micro-HDMI port (some bundles include adapters — confirm per listing).</li>
    <li>Status: Finalized.</li>
  </ul>

<h1>Power</h1>
  <p><em>4 jobs: store energy, charge safely, protect from over-discharge, convert voltage for each board.</em></p>

  <h2>Battery Cells</h2>
    <p><a href="https://www.nealsgadgets.com/products/samsung-inr18650-35e-battery">Samsung INR18650-35E (x2)</a></p>
    <ul>
      <li>Qty: 2, wired in parallel (NOT series — must read "3.7V," not "7.4V")</li>
      <li>Cost: $6.95-13.60</li>
      <li>Spec: 3500mAh, 8A continuous discharge each → ~7000mAh / 16A combined</li>
      <li>Purpose: Main energy storage. 18650 format, flat-top, unprotected (protection handled separately by BMS below).</li>
    </ul>
  <h2>Battery Holder</h2>
    <p><a href="https://artofcircuits.com/product/18650-3-7v-battery-holder-for-3-cells-with-wires">2-cell 18650 parallel holder</a></p>
    <ul>
      <li>Qty: 1 (2-cell version)</li>
      <li>Must be labeled "3.7V" (parallel) — NOT "7.4V"/"11.1V" (series)</li>
      <li>Check wire lead gauge on arrival — thin leads (22-24AWG) are only rated ~3A; may need to upgrade to 18-20AWG wire to safely carry ~5A peak load.</li>
    </ul>
  <h2>Charging (charge-side only)</h2>
    <p><a href="https://www.addicore.com/products/tp4056-tc4056a-lithium-battery-charger-and-protection-module?variant=45759528534333">TP4056 w/ Protection, USB-C</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $1.</li>
      <li>Wire to BAT+/BAT- only — do NOT run system load through its OUT pins (limited to 3A, below our ~5.3A peak need).</li>
      <li>Only rated for up to 2 cells in parallel — matches our 2-cell plan exactly.</li>
    </ul>
  <h2>Discharge Protection</h2>
    <p><a href="https://www.aliexpress.us/item/2255800112182626.html?gatewayAdapt=nld2usa4itemAdapt">1S 3.7V 6A 4MOS BMS</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $0.99-1.78</li>
      <li>Purpose: Sits between battery pack and buck-boost converters. Handles discharge-side over-current/over-discharge cutoff at a rating that actually matches system draw.</li>
    </ul>
  <h2>Power Conversion — 5V rail (Orange Pi)</h2>
    <p><a href="https://quartzcomponents.com/products/tps63020-automatic-buck-boost-step-up-down-power-supply-module-5v-lithium-battery-low-ripple-voltage-converter">TPS63020 Buck-Boost Module, 5V fixed output</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: $3.02</li>
      <li>Input: 1.8-5.5V (covers full 3.0-4.2V battery range) → Output: fixed 5V, up to 3A, 96% efficiency</li>
      <li>Status: Confirmed.</li>
    </ul>
  <h2>Power Conversion — 3.3V rail (ESP32s + radio modules)</h2>
    <p><a href="https://www.amazon.com/JESSINIE-TPS63020-Automatic-Buck-Boost-Lithium/dp/B0CB3WKY1Y">TPS63020 Buck-Boost Module, 3.3V fixed output</a></p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$5-8</li>
      <li>Input: 1.8-5.5V → Output: fixed 3.3V, up to 3A</li>
      <li>Powers: both ESP32-S3s, CC1101, PN532, RDM6300, NRF24L01</li>
      <li>Status: Confirmed.</li>
    </ul>
  <h2>NRF24L01 Brownout Fix</h2>
    <p>10-100µF electrolytic/tantalum capacitor</p>
    <ul>
      <li>Qty: 1</li>
      <li>Cost: ~$1</li>
      <li>Purpose: Placed directly across NRF24L01+PA+LNA power pins to absorb current spikes (~115mA bursts) and prevent random resets/brownouts — a well-known fix for this specific module.</li>
    </ul>

  <h3>Simple flow</h3>
  <pre>
[2x Samsung 35E, parallel]
        |
        +--> [TP4056] (charging only, plug in here)
        |
        +--> [BMS] --> [TPS63020 #1: 5V]  --> Orange Pi
                    --> [TPS63020 #2: 3.3V] --> ESP32-S3 x2, CC1101, PN532, RDM6300, NRF24L01
  </pre>

<h1>Enclosure / Misc</h1>
  <ul>
    <li>3D printed case (6" x 8" x 1.5-2") — filament cost, ~$10-20</li>
    <li>Perfboard/protoboard — ~$5</li>
    <li>Wiring, headers, connectors, switches — ~$15-20</li>
  </ul>
