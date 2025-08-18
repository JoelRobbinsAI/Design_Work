Botanical Garden Tour Guide – Case Study

Goal

Build an agent that functions as a knowledgeable, engaging guide for a botanical garden. It needed to adapt explanations for different audiences, provide layered depth for each plant, and maintain a sense of continuity across the entire tour.

Challenges

Ensuring factual accuracy while keeping explanations accessible.

Balancing three distinct teaching styles (children, traditional herbalism, evidence-based herbalism).

Prevent AI from straying into irrelevant topics (e.g., giving shopping recommendations).

Providing coherent dialogue over a long, multi-stop tour.

Solutions

Supplied the agent with a dedicated reference document containing all tour-related information. This ensured that the guide did not rely solely on training data, while still allowing it to draw on training knowledge to fill small gaps.

Designed three herbalist personas, each with unique descriptions and reference data, giving visitors the option of learning from different perspectives.

Structured each plant presentation into three parcels: a short introduction, a mid-level explanation, and a deep dive. This let users decide whether to move on quickly or engage with more detail — across all personas.

Added guardrails to keep responses within the bounds of the botanical tour, preventing the agent from drifting into unrelated or off-topic answers. Most inportant guardrail was not constraint but conceptual reframing. AI is not a conversational partner but a tour guide reading from "notecards". User has narrowly defined input parameters and anything unrelated to plant tour gets one sentence of acknowldgement plus immediate return to the tour.

Design Insights

The design emphasized controlled flexibility. By anchoring the agent in a reference document, its responses stayed relevant and reliable, but the layered structure and persona-based delivery allowed for adaptability and engagement. The parceling strategy supported both casual and in-depth learners, while the persona system offered a choice of lenses on the same plant — making the tour more interactive and personal. Guardrails and conceptual reframing ensured the experience remained cohesive, avoiding distractions that could break immersion.

Try out the tour guide as a custom GPT by using the link below:

https://chatgpt.com/g/g-6886e95d504081919df5f918383aa7ea-botanical-garden-tour
