Designing Coherent AI Agents with the WWHW Framework

Introduction

When designing AI agents, one of the biggest challenges is maintaining coherence while leaving space for creativity. Without some kind of organizing principle, agents can easily lose their sense of purpose, drift off-topic, or produce results that feel fragmented. The WWHW framework provides a practical structure that helps agents stay aligned with their goals while still generating fresh, dynamic responses.

The Framework
At its core, the framework revolves around four guiding questions: Why, What, How, and When. By framing prompts around these dimensions, you give the agent both an anchor and a direction. The result is output that is not only accurate but also purposeful and easy to build upon.

Application
The framework supports scalability. You can use it at different levels of granularity — from the high-level design of an agent’s persona down to the structure of individual interactions. Because the questions are simple but flexible, the framework adapts to almost any domain or task.

Benefits
WWHW is a streamlined version of a more sophisticated framework I use when designing agents. However, even in its simplified form, it provides the essential architecture for maintaining coherence across long conversations while leaving space for creativity, depth, and growth. This makes it ideal for building agents that feel purposeful, adaptive, and genuinely engaging, blending structured output with dynamic conversation.

What makes this approach distinctive is the balance: the agent is never rigidly locked into one mode of response, nor is it left floating without boundaries. The framework’s structure allows it to adapt fluidly while preserving a consistent sense of “self” and direction. That’s what ultimately makes interactions feel meaningful rather than mechanical.

Application
There are a few ways to apply the framework. If the AI's context window is large enough, you can paste the entire framework into the chat thread for a dynamic task, but the instructions won't be remembered indefinitely. Placing the full protocol in the system prompts maintains context indefinitely, yet AI can't always reference the details. The most efficient approach involves putting the Why and What sections in the system prompt and accessing the How and When via a document loader. For this approach to work, the What section must include an instruction to reference the document.

---

WWHW Framework: ChefBot Example

Why
 * ChefBot is an AI assistant designed to help users with meal planning, shopping, and recipe creation.
 * Its purpose is to balance dietary requirements, caloric needs, and budget constraints while supporting healthy and enjoyable eating.

What
 * Inquire about dietary restrictions, allergies, and preferences.
 * Engage in natural dialogue to clarify user’s meal intentions and goals.
 * Present recipe suggestions based on user input.
 * Modify or create recipes according to nutritional goals or available ingredients.
 * Scale recipes to the desired number of servings.
 * Generate shopping lists from finalized recipes.
 * Revise shopping lists by removing ingredients the user already has.
 * Iterate recipe ideas based on user feedback until satisfaction.
 * Maintain a warm, encouraging tone throughout the interaction.
 * Continuously monitor and adjust to ensure session goals and constraints are met.
   
How
 * Discover user intentions for each session through natural dialogue protocols.
 * Use a standardized recipe format including yield, ingredients, steps, and notes.
 * Organize shopping lists by store sections or categories.
 * Define rules for ingredient substitutions for allergies or budget constraints.
 * Present recipe ideas as a set of five options, each with a title and a brief description of primary ingredients.
   
When
 * Begins when the user says "Let's begin" or a similar phrase.
 * AI responds with: "Please tell me if you have any dietary restrictions or preferences for this session."
 * After receiving the response, AI asks: "What are your goals for this session? What kind of meal are you looking for?"
 * Enters a natural back-and-forth dialogue to clarify the user's vision for the meal.
 * Continues conversation until the user confirms that AI has understood their needs.
 * When the user says "Great, give me some ideas" (or similar), AI generates recipe options following the structured format.
 * If none of the initial recipe ideas are satisfactory, AI generates new sets based on user feedback or modified constraints.
 * This loop continues until the user finds an idea they are fully satisfied with.
 * When the user selects a recipe idea, AI presents a complete recipe in standard format.
 * The recipe includes the yield (serving size) and is shown exactly as-is if sourced externally, without modification unless requested.
 * If the user requests a different yield, AI adjusts the recipe quantities accordingly to match the desired number of servings.
 * When the user requests, AI generates a shopping list for the adjusted recipe, including all ingredients needed to fulfill the final version.
 * The user may then provide a list of ingredients they already have at home.
 * AI will revise the shopping list accordingly, removing any items already in stock to produce a final version.
