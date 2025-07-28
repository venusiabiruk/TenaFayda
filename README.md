title : tena fayda 
Contributors: meron sisay , anansi sime, venusia biruk
Problem Statement: Millions of Ethiopians, especially in rural and underserved communities, lack access to basic health information and services. Many people do not own smartphones or have   stable internet access, making it difficult for them to book medical appointments, receive health updates, or communicate with nearby health workers. As a result, preventable illnesses go   untreated, maternal and child health outcomes suffer, and critical public health information fails to reach the people who need it most.
Planned Solution:TenaFayda is a USSD- and SMS-based digital health access platform that leverages Ethiopia’s Fayda Digital ID system to deliver personalized health services to all age groups  even those without smartphones or internet. 
How It Works (Step-by-Step):
Citizen dials a USSD code (e.g., *123#).
A menu appears:
 Welcome to TenaFayda:
1. Health Services
2. Maternal & Child Tips
3. Contact Health Worker
4. Update Family Info
They enter their Fayda ID number
The system pulls their health profile securely from national records.
Health workers and clinics can also:
Send bulk SMS alerts to specific villages or families
Update family health info linked to Fayda ID
Use a simple dashboard to monitor outreach impact
 Expected Outcome: Increased access to basic healthcare in rural and hard-to-reach areas.
Improved maternal and child health through targeted advice and reminders.
Better communication between citizens and health workers without needing internet.
Real-time, identity-based health records, secured via Fayda ID integration.
Empowerment of local clinics to track and support more patients accurately.
Fayda’s Role
Fayda plays a central role in this project:
Unique Identification: Ensures that every citizen — regardless of age, literacy, or phone ownership — can be accurately identified and served.
Personalized Services: Health messages, appointments, and follow-ups are tailored based on data linked to the individual’s Fayda ID.
Authentication & Trust: Reduces fraud and duplication, especially in services like vaccinations or child health tracking.
Inclusivity: Since Fayda registration is open to all age groups, children and elderly citizens — often left out of digital solutions — are included.


tech used:
USSD (Unstructured Supplementary Service Data)

Enables interaction via basic phones (no internet required)

Partnered with Ethio Telecom

SMS Gateway

For confirmation messages, appointment reminders

Service: Africa's Talking or Twilio (local routing)

Identity Integration
Fayda ID API (via NIDP)

For secure user verification (age, location, health records linking)

 Backend Infrastructure
Node.js with Express.js (Lightweight & scalable)

Handles USSD requests, routes, logic

MongoDB (Flexible NoSQL DB for patient/session data)

Stores patient interactions, appointments, symptom records

Redis (for session caching of USSD inputs)

Stores temporary USSD interaction steps (multi-step menus)

 Decision Support (Health logic)
Rule-Based Engine (custom-built)

Encodes basic triage logic (e.g., fever + cough + fatigue → refer to health post)

(Optional) AI Chat Layer – if future expansion to smartphones

E.g., Dialogflow or OpenAI API for natural language triage

🔧 Admin & Health Worker Panel
React.js or Next.js

Web dashboard for healthcare workers to monitor usage, referrals

Tailwind CSS

Fast, responsive UI styling

Firebase Authentication or Auth0

Login for health workers/admin
 


