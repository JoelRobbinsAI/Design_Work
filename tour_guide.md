Botanical Garden Tour Guide – Case Study

[Take a virtual tour with my tour guide agent!](https://chatgpt.com/g/g-6886e95d504081919df5f918383aa7ea-botanical-garden-tour)

Goal

Create an interactive agent that guides users through a botanical garden experience. The agent needed to deliver engaging, accurate plant education tailored to different audiences, while maintaining a sense of narrative flow across multiple stops on the tour.

Challenges

Balancing factual depth with accessibility

Supporting three distinct teaching styles (child-friendly, traditional herbalist, evidence-based)

Preventing the model from drifting into unrelated topics

Maintaining continuity across a long-form, multi-plant conversation


Solutions

I provided the agent with a dedicated reference document containing all tour content, ensuring it could deliver grounded responses without relying too heavily on training data. The guide could still draw from general knowledge to fill minor gaps.

I designed three narrator personas: an elder herbalist, a kid friendly herbalist, and a science-based herbalist. Each had a defined tone and voice. Tour stops were structured with three sets of narratives per plant. The user could listen to all three or move on at any time, giving them control over how deeply they wanted to engage with each plant, and which perspective they preferred.

Instead of toggles or branching logic, I embedded all behavior control in the prompt itself. The agent treats user messages as cues to shift persona or advance the tour. For example, if a user says “next plant in a kid’s voice,” the guide switches seamlessly. This eliminated the need for any parsing or logic chains.

I also included guardrails by reframing the agent’s role. It is not a conversational partner, but a tour guide reading from prepared notecards. If a user goes off-topic, the agent offers a one-sentence acknowledgment, then gently returns to the tour.

Design Insights

The design emphasizes clarity and adaptability. Anchoring the agent in a reference document kept answers focused and consistent. The layered explanation format supported both casual and deep learners. The persona design allowed users to choose how they wanted to engage without complicating the backend logic. Overall, the system provides flexibility within clear boundaries, preserving immersion and coherence.

[See a walkthrough video of this agent](https://youtu.be/T7zNl-zhaVw?si=FusoXFn1KKJ2g8ue)

[Try out the tour guide agent created with Flowise](https://cloud.flowiseai.com/chatbot/249394e7-66cb-44d9-9f4d-67bd32568929)

[Try out the tour guide agent as a Gem!](https://gemini.google.com/gem/791cbe7320ac/81ec116e59d2e1b7)
