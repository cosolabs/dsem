# Case study: Public building, 6000 m², zero budget (2021-2024)

**Author:** In-house R&D team (anonymized)  
**Period:** 2021-2024  
**Building size:** 6000 m²  
**Context:** Public sector, complete budget cut for infrastructure maintenance

---

## The challenge

In 2021, the maintenance budget for a 6000 m² public building was reduced to zero. The building housed:

- A **data center** distributing national public signals
- **Offices** with 200+ daily occupants
- **Critical infrastructure**: water tanks, sewage pumps, HVAC systems

No money meant:
- No new hardware
- No external contractors
- No paid software licenses
- No spare parts

**The only available resources:**
- Discontinued components from old programs
- Recycled hardware
- Open source software
- In-house engineering knowledge

---

## The six layers (in chronological order)

### Layer 1: Data center monitoring

**Problem:** The data center (hosting national public signals) had no monitoring. If temperature or humidity exceeded safe ranges, nobody would know until servers failed.

**Solution:** First version with **OpenHAB + ESP32** using recycled sensors.

**What it validated:** D1 (open infrastructure), D2 (zero dependency), D7 (sustainability), D8 (local data)

---

### Layer 2: OpenHAB doesn't scale

**Problem:** As we added more devices and logic, OpenHAB showed its limits.

**Solution:** Custom stack built with:
- **Mosquitto (MQTT)** for message transport
- **Node-RED** for business logic
- **InfluxDB** for time-series data
- **Grafana** for visualization

**What it validated:** D1 (open standards), D5 (structural complexity), D7 (sustainability)

---

### Layer 3: Water tanks (12,000 liters total)

**Problem:** Two 6000-liter tanks (one gravity-fed, one with pressure pumps) had no monitoring. Small leaks or stuck float valves could waste thousands of liters undetected.

**Solution:** Sensors + night pattern analysis in Node-RED. The system learned what "normal" looked like at night (when the building was empty) and alerted on anomalies.

**What it validated:** D3 (functional depth), D5 (structural complexity)

---

### Layer 4: Sewage pumps (sanitary risk)

**Problem:** Sewage pumps could burn if something got stuck. A burned pump meant **the building couldn't evacuate waste** — a sanitary crisis.

**Solution:** Time-based protection in Node-RED. The system learned normal pump cycles and automatically shut down any pump running longer than expected, triggering an alert.

**What it validated:** D2 (operational dependency), D3 (functional depth), D7 (sustainability)

---

### Layer 5: Rooftop HVAC (common areas)

**Problem:** Rooftop AC units in common areas could be turned on by anyone and left running all weekend. No control, no schedules, no accountability.

**Solution:** 10 custom thermostats built with ESP32, connected to the stack, without modifying original wiring. Added schedules, occupancy logic, and remote monitoring.

**What it validated:** D1 (infrastructure), D3 (functional depth), D5 (structural complexity)

---

### Layer 6: Emergency doors (behavioral problem)

**Problem:** Emergency exits were being used as shortcuts, bypassing the external biometric access system. Doors wore out, security was compromised.

**Solution:** Magnetic sensors on doors + alerts. No changes to the biometric system. Staff KNEW doors were monitored — and stopped misusing them.

**What it validated:** D1 (infrastructure), D3 (functional depth), D6 (transparency)

---

## What we learned (dimension by dimension)

### D1 — Infrastructure
When everything is open, nothing ties you down. You can change platforms, recycle hardware, modify logic. When budget disappears, the only thing left is what you can maintain yourself.

### D2 — Operational dependency
Zero dependency is not a luxury. It's the only way to survive when the context is uncertain. If we had bought a closed system, today there is no monitoring.

### D3 — Functional depth
Depth is not the number of devices. It's how many different systems you can make talk to each other and to the central logic. Each new layer multiplies the value of the previous ones.

### D4 — Value model
When the budget is zero, hardware stops mattering. The only thing that counts is what you can do with what you have.

### D5 — Structural complexity
Complexity isn't in civil works. It's in understanding how each system works to add intelligence without breaking it. That's harder than new construction.

### D6 — Technological transparency
Transparency isn't just "showing". It's that people know that what they do has visible consequences. That changes behavior.

### D7 — Sustainability over time
Sustainability isn't "buying something that lasts". It's choosing technologies with community, with standards, with alternatives. What depends on a company, dies with it.

### D8 — Privacy and data sovereignty
When your data is yours and on your network, no one can take it, no one can charge you to see it, no one knows what happens in your building. In an uncertain context, that's peace of mind.

---

## Conclusion

This project ran for three years (2021-2024) with exactly **zero budget** for hardware, software, or external contractors.

It survived because:
- Every component was based on **open standards**
- Every decision prioritized **zero dependency**
- Every layer was built to be **maintainable by the team**

DSEM doesn't describe a theoretical ideal. It describes what actually worked when there was no other option.

> If this worked in a public building with everything against it, it can work anywhere.

---

**Anonymized case study — March 2025**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
