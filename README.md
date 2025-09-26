✈️ Salesforce Airline Management System (AMS)


Developer Edition –  Org Project


A Salesforce-based Airline Management System (AMS) designed and implemented on Developer Edition (Free). The project simulates a lightweight CRM solution for airlines, focusing on ticket booking, passenger management, flight scheduling, and refunds — optimized to fit within free org limits.


🛑 Problem Statement


Airlines face challenges in efficiently managing day-to-day operations such as flight scheduling, ticket booking, passenger data management, and handling cancellations/refunds. Traditional systems are often siloed, making it difficult for agents and administrators to track real-time information. Passengers also face delays in updates, lack of transparency in booking/refunds, and poor customer experience.


Key challenges:

• Manual and fragmented booking process.

• Difficulty in tracking flight schedules and seat availability.

• Inefficient management of passenger information.

• Complex and time-consuming refund requests.

• Limited visibility for stakeholders in a single platform.


⸻


✅ Solution (using Salesforce Developer Edition)


To overcome these challenges, we propose an Airline Management System (AMS) built on Salesforce CRM. The solution leverages Salesforce’s cloud-based platform to centralize and automate processes, ensuring real-time access, better transparency, and improved customer experience.


Core Features of the Solution:

1. Flight Scheduling Management

• Custom objects for Flights, Routes, and Schedules.

• Real-time updates for flight timings and availability.

2. Ticket Booking System

• Booking agents can create and manage bookings directly in Salesforce.

• Automation rules to confirm seats and generate booking records.

3. Passenger Information Management

• Store passenger details under Contact records.

• Easily track travel history, bookings, and preferences.

4. Refund & Cancellation Handling

• Workflow/Approval process for refund requests.

• Automated status updates to agents and passengers.

5. Dashboards & Reports

• Admin dashboards for total bookings, flight occupancy, and cancellations.

• Agent dashboards for managing assigned passengers and flights.


⸻


🎯 Expected Benefits

• Streamlined booking and scheduling process.

• Centralized passenger database with easy access.

• Reduced manual errors and faster refunds.

• Better decision-making with real-time dashboards.

• Improved customer experience and airline efficiency.

⸻


📌 Phase 1: Problem Understanding & Industry Analysis


Scope:

• Ticket Booking

• Flight Scheduling

• Passenger Management

• Refund Requests


Stakeholders:

• Admin (System Owner)

• Booking Agent (Internal Salesforce User)

• Passenger (Contact Records only, no login access)


Assumptions:

• Single airline (Skyline Airlines).

• Limited demo routes and flights.


⸻


📌 Phase 2: Org Setup & Configuration

• Edition: Salesforce Developer Edition (Free).

• Company Profile → Skyline Airlines.

• Users → Admin + 1 Booking Agent.

• Roles & Profiles: Admin, Airline Staff (Agent).

• OWD: Flights = Public, Bookings = Private.

• Change Management: No sandbox → use Unmanaged Package/Change Sets.


⸻


📌 Phase 3: Data Modeling & Relationships


Custom Objects:

• ✈️ Flight

• 🎟️ Booking

• 💳 Ticket

• 💰 Payment


Standard Object Extension:

• 👤 Passenger → Contact (with custom fields: Passport No., DOB, Nationality).


⸻


📌 Phase 4: Process Automation

• Validation Rules → Prevent overbooking (capacity check).

• Flows →

• Auto-create Ticket on Booking confirmation.

• Send booking confirmation email.

• Auto-cancel Booking if Payment not received within 24 hrs.


⸻


📌 Phase 5: Apex Programming

• Triggers:

• Update available seats after Booking.

• Prevent duplicate bookings.

• Batch Apex: Archive old flights.

• Future Method: Async notifications (demo).

• Test Classes: >75% coverage.


⸻


📌 Phase 6: User Interface

• Lightning App: Airline Agent Console.

• Record Pages: Passenger 360° view (Bookings, Tickets, Payments).

• LWCs:

• Flight Search.

• Seat Selection (demo).

• Flight Status Board.


⸻


📌 Phase 7: Integration

• REST Apex Class → Book Flight API (demo).

• Platform Events → Flight Delay Alerts.

• Mock external payment system (not live).


⸻


📌 Phase 8: Data Management

• Demo data: 10 Flights, 20 Passengers, 15–20 Bookings.

• Duplicate Rules for Passengers.

• Backup: Unmanaged Package.


⸻


📌 Phase 9: Reporting & Security


Reports:

• Bookings by Flight

• Revenue by Flight

• Passenger Trends


Dashboards:

• Flight Occupancy

• Monthly Revenue


Security:

• Role Hierarchy: Admin > Agent

• Audit Trail enabled


⸻


📌 Phase 10: Demo & Presentation


End-to-End Demo Flow:

• Passenger record → Booking → Ticket auto-created → Payment recorded.

• Automated Flows + Apex execution.

• Dashboards: Flight Occupancy & Revenue.


Deliverables:

• ERD Diagram

• Flow Screenshots

• Apex Code (Triggers, Batch, REST, Tests)

• Dashboards
