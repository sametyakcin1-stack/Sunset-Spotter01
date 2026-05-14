# Sunset-Spotter01
Phase 1: The Topic Marketplace (The Niche)
For this project, I moved away from generic utility suggestions to focus on a hyper-local experience: the İzmir sunset. While the city is famous for its coast, the "perfect" spot depends on highly specific variables.

The Problem: Most people default to the same crowded spots in Kordon, missing out on diverse atmospheres that better suit their current mood or logistics.

Target Audience: Specifically designed for university students in İzmir and young locals who want to optimize their evening based on their mode of transport, budget, and desired "vibe."

The Niche: Unlike a general map, this app acts as a local "insider," categorizing spots by their specific sunset "characteristics"—ranging from the bustling urban energy of Karşıyaka to the quiet, elevated views of the Historical Lift (Asansör).

Phase 2: From Matrix to Code (The Technical Build)
The development process was driven by a strict logic matrix. Before any code was written, I mapped out every possible user journey using a Mermaid flowchart to ensure there were no "dead ends."

Interface & Interaction: The app utilizes a clean, single-page interface built with HTML5 and CSS3. I chose a minimalist design to keep the focus on the visual output. The interaction is driven by dynamic buttons and selection menus, ensuring a smooth user experience.

The Decision Logic: To meet the project requirements, the app features five key decision points:

Transport Mode: (Walking, Public Transit, or Car)

Budget: (Free/Public Space vs. Paid/Cafe setting)

Atmosphere: (Quiet/Secluded vs. Social/Lively)

Elevation: (Sea level vs. Rooftop/Hilltop)

Time Constraints: (Quick access vs. Worth a long commute)

AI Collaboration: I acted as the "Project Manager" for the AI (Gemini/ChatGPT). Instead of asking it to "build an app," I provided my Conditions Table and Variable Definitions first. I fed the AI the specific logic strings (e.g., IF Transport=Walk AND Budget=Zero AND Vibe=Social THEN Result=Bostanlı Sahil) and instructed it to generate the JavaScript if/else structures based strictly on that matrix.

Phase 3: Build-Log Reflection (Technical Insights)
The Logic Breakdown
The most complex "branch" of the code involved balancing the Transport and Elevation variables. For instance, if a user wants an elevated view (like Seyirtepe) but has no car, the logic must prioritize accessibility via public transit or suggest a closer alternative like Varyant.

Code Walkthrough
The "intelligence" of the app resides in a centralized JavaScript function. This function captures the values from the interactive buttons and runs them through a series of conditional statements. The innerHTML property is then used to display the final recommendation, including a description of why that spot fits the user's specific criteria.

Problem-Solving & Reflection
The most challenging part of the build was "debugging" the AI's tendency to simplify the logic. During initial drafts, the AI occasionally skipped certain variables to make the code shorter. I had to intervene by re-prompting with my Mermaid flowchart, forcing the code to respect the specific "niche" constraints I had set in Phase 1. This ensured that the final product was not just a generic script, but a reflection of my unique logic matrix.
