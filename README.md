# Household Energy Consumption Cost Estimator

## Project Overview
A single-screen Flutter mobile application designed to estimate daily and monthly electricity consumption costs for household appliances. The application operates entirely without an external database, maintaining user inputs dynamically in temporary runtime memory.

---

## Technical Specifications & Features
* **Language/Framework:** Dart / Flutter
* **Architecture:** Single-Screen `StatefulWidget` (In-Memory `List<Appliance>`, No Database)
* **Core Functionality:**
  * **Custom Rate Configuration:** User-defined electricity cost per kilowatt-hour ($/kWh).
  * **Dynamic Appliance Management:** Feature to add custom appliances with specific names, wattage inputs, and daily usage hours.
  * **Interactive List Display:** Table view displaying active appliances and individual daily runtime inputs.
  * **Real-Time Calculation Engine:** Instant calculation of daily and monthly (30-day) overall energy costs using Flutter's state management (`setState`).

---

## Cost Calculation Logic
The application processes energy usage using the standard kilowatt-hour formula:

$$\text{Daily Cost} = \left(\frac{\text{Wattage (W)} \times \text{Daily Hours}}{1000}\right) \times \text{Electricity Rate (\$/kWh)}$$

$$\text{Monthly Cost} = \text{Daily Cost} \times 30$$

---

## Project Structure & Task Distribution (Solo Developer)
Since this project is developed individually, tasks are categorized into two structured development phases:

* **Phase 1: Front-End UI & Widget Design**
  * Flutter widget tree layout design.
  * Single-screen input controls (`TextField` for rates/inputs, `ListView` for appliances, `ElevatedButton`).
  * Interface formatting and calculation output container.

* **Phase 2: Application Logic & State Management**
  * In-memory state storage using dynamic Dart lists (`List<Appliance>`).
  * Event handlers for dynamic appliance addition and reactive updates (`setState()`).
  * Mathematical processing engine for daily and monthly cost estimations.
---

## Project Info
* **Course:** CSCI410 Mobile Application Development
* **Developer:** Yasmin Kassem
* **Submission Date:** November 12
