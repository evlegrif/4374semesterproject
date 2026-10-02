Technical Risks:
    T-01: Push Notifation Failure - Errors integrating with Apple or Google notifcation services prevent session ending alerts 
    T-02: GPS Handoff Failure - Parking spot GPS coordinate is inaccurate or handoff URL scheme is broken and either does not work or leads drivers to incorrect locations
    T-03: Database Double Bookings - High traffic spikes may cause race conditions in the databsae, leading to two or more drivers being able to book a singular spot
    T-04: ALPR Hardware Latency - ALPR cameras at garage gates experience network lag and do not transmit the packets when communicating with the backend, which could delay gate openings or desync capacity counts

Schedule Risks:
    S-01: Extended Time Needed for Audits - Municipal legal review and compliance verification takes longer than anticipated or delayed due to external factors, leading to less time for the QA team
    S-02: App Store Rejections - Apple or Google app stores may reject the app for any number of reasons, delaying the release of the app
    S-03: Backend API Delays - Backened completion of infrastructure is delayed, and the REST APIs block the Web and Mobile App teams from starting their respective integrations
    S-04: Holiday Time off - Our current schedule runs through Thanksgiving break, where many of our American workers will likely take some time off. 

Financial Risks: 
    F-01: Cloud and API Consumption Creep - Although the budget is unlimited, should the maintainence budget be capped, the cost over time could increase outside of the initial scope
    F-02: ALPR Chargebacks - ALPR cameras cannot be 100% accurate and might overcharge for extended stays ,resulting in refunds and chargeback fees
    F-03: Regulatory Fines for Data Breaches - If vehicle data is not encrypted to legal standard, legal penalties might ensue
    F-04: SMS/Push Notifications Overage - Notification loops could trigger thousands of duplicate texts or pushes, generating massage usage bills from AWS

People Risks: 
    P-01: Head Developer Unavailability: Loss or temporary unavailability of lead engineers on the project will stall critical paths
    P-02: Operator Training Resistance - Parking staff might be unfamiliar with the technology and dynamic pricing leading to operational errors
    P-03: QA Bottleneck - QA testing does not go as planned and causes delays in development
    P-04: Team Misaligment - Poor communication between different teams resulting in mismatching application structures, requiring rework and time extensions