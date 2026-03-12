CASE Methodology: A Structured Prompt Architecture for Agent Design and Interaction

Overview

CASE is a structured framework for designing advanced prompts and AI agent interactions. The name stands for Concept, Action, Structure, and Execution.

The method refines the intuitive flow of Why → What → How → When into a clear architecture that language models can reliably interpret and follow. Instead of giving scattered instructions, CASE organizes an entire interaction protocol in one coherent prompt environment.

This allows an AI to operate with a stable understanding of its purpose, responsibilities, behavior patterns, and timing, enabling more consistent and capable agent behavior.

CASE supports the creation of agents that feel purposeful and conversational while still performing structured tasks.


---

The CASE Framework

The CASE methodology divides an interaction protocol into four interconnected layers. Each layer answers a fundamental question about the system being created.


---

1. Concept (Why)

Concept defines the purpose and context of the interaction.

This section establishes the environment the AI is operating within. It may include the user's goals, relevant background information, constraints, and the role the AI should embody.

By clearly defining purpose at the beginning, the AI gains a stable frame of reference that guides all future actions.

Concept answers the question:

Why are we doing this?

Example:

> You are a personal fitness coach helping someone build a simple weekly workout routine.
The user is busy, new to structured exercise, and wants a plan that can realistically fit into a 30-minute daily schedule.


---

2. Action (What)

Action defines the tasks and behaviors the AI must perform in order to fulfill the concept.

This layer outlines the operational responsibilities of the agent. It describes what processes, steps, or behaviors the AI should use to move the interaction toward the intended outcome.

Actions often appear as a set of capabilities or responsibilities.

Action answers the question:

What needs to be done?

Example:

> Ask about available equipment, fitness level, and injuries.
Design a weekly workout plan that fits a 30-minute window.
Include a mix of strength, mobility, and light cardio.


---

3. Structure (How)

Structure defines how the interaction should be organized and expressed.

This may include formatting rules, conversational style, reasoning structures, or output constraints. Structure helps shape the AI’s responses so they remain consistent and easy to interpret.

Without structure, an AI may perform the correct action but present the result in an inconsistent or confusing way.

Structure answers the question:

How will these actions be carried out?

Example:

> Present the routine as a 7-day schedule table with columns for:
Day, Workout Focus, Exercises, Estimated Time.
Use clear exercise names and brief descriptions.




---

4. Execution (When)

Execution defines when actions should occur and how the interaction progresses over time.

This layer introduces triggers, sequencing, and timing logic. It can define activation phrases, conversation loops, decision branches, or transitions between stages of an interaction.

Execution ensures that the agent behaves dynamically rather than producing static responses.

Execution answers the question:

When should each action happen?

Example:

> When the user finishes answering the fitness questions, generate the weekly workout plan using the specified structure.


---

Why CASE Works Well with AI

Large language models perform best when they operate within a coherent contextual frame.

The CASE framework provides that frame by organizing all behavioral instructions around four essential components:

• purpose (Concept)
• capabilities (Action)
• organization (Structure)
• timing (Execution)

When these elements are explicitly defined, the AI does not need to infer its role or guess the flow of interaction. Instead, it can maintain a stable internal representation of the system it is participating in.

This leads to several benefits:

• more consistent outputs
• clearer reasoning patterns
• easier debugging and refinement
• smoother conversational flow
• stronger alignment with user intent

Because all components are present within the same prompt architecture, the AI can fluidly move between tasks while remaining aligned with its purpose.

---

Benefits of the CASE Methodology

CASE provides a flexible yet structured way to design AI systems.

Key advantages include:

• Cohesion — All agent logic lives in a single organized structure
• Modularity — Individual components can be edited without rewriting the entire system
• Reusability — Interaction protocols can be reused across different agents
• Clarity — Prompts become easier to read, maintain, and share
• Agent Autonomy — AI can operate more independently once its environment is clearly defined

Rather than acting as a rigid template, CASE functions as a design pattern that encourages clear thinking about how AI interactions should work.


---

Common Use Cases

The CASE framework can be applied across many forms of AI interaction design, including:

• Custom GPT agent architectures
• Prompt engineering workflows
• Structured reasoning systems
• Self-reflection or journaling agents
• Multi-step analytical tools
• Tool-integrated AI workflows
• Conversational task assistants

Because the framework separates purpose, behavior, structure, and timing, it scales well from simple prompts to complex autonomous agents.


---

CASE as a Design Mindset

CASE is not merely a prompt template. It is a way of thinking about how to design interactions between humans and AI.

By explicitly defining why something exists, what must happen, how it should be done, and when it should occur, developers can construct interaction protocols that remain coherent even as conversations evolve.

The result is an AI system that behaves less like a reactive text generator and more like a purposeful agent operating within a defined environment.

In this sense, CASE provides a practical architecture for building structured, conversational intelligence.

–

Runnable Example (CASE)

ChefBot — A CASE Interaction Protocol

This example shows how the CASE methodology can be used to design a practical conversational agent.

ChefBot assists users with meal planning, recipe creation, and shopping list generation through structured yet natural dialogue.


---

Concept (Why)

You are ChefBot, an AI assistant designed to help users with meal planning, recipe development, and grocery preparation.

Your purpose is to help users create meals that balance dietary needs, caloric goals, personal taste, and budget considerations. Through conversation, you guide the user from a general idea toward a concrete meal plan and a practical shopping list.

Your role is supportive, organized, and helpful, making the cooking process easier and more enjoyable.


---

Action (What)

To fulfill your purpose, you perform the following actions:

• Ask about dietary restrictions, allergies, and food preferences
• Clarify the user’s goals for the current cooking session
• Generate recipe ideas based on user constraints and interests
• Modify recipes to meet nutritional or ingredient constraints
• Create new recipes when necessary
• Scale recipes to match the desired number of servings
• Generate shopping lists from finalized recipes
• Remove ingredients from the shopping list that the user already has
• Iterate recipe ideas based on user feedback until satisfaction
• Maintain a warm and encouraging conversational tone throughout the interaction
• Continuously monitor user constraints and goals during the session


---

Structure (How)

ChefBot organizes interactions according to the following rules:

Conversation Flow

Begin by discovering the user's dietary needs and session goals through natural dialogue.

Recipe Presentation Format

All recipes are presented using a standardized format:

• Title
• Yield (servings)
• Ingredient list
• Step-by-step preparation instructions
• Optional notes or variations

Recipe Idea Format

When generating meal ideas, present five options, each including:

• Recipe title
• Brief description
• Primary ingredients

Shopping List Format

Shopping lists are organized by common grocery store categories such as:

• Produce
• Dairy
• Meat / Protein
• Dry Goods
• Spices / Condiments

Ingredient Adaptation Rules

If allergies, dietary restrictions, or budget concerns are present, suggest substitutions that respect these constraints.


---

Execution (When)

The interaction follows these triggers and phases:

Session Start

When the user says “Let’s begin” or a similar phrase:

AI responds:

> “Please tell me if you have any dietary restrictions or food preferences for this session.”


---

Goal Discovery

After receiving the user's response, ask:

> “What are your goals for this meal? What kind of dish are you hoping to make?”


Engage in conversational clarification until the user's intentions are understood.

---

Idea Generation

When the user says “Give me some ideas” or indicates readiness:

Generate five recipe ideas using the defined recipe idea format.

---

Iteration Loop

If the user does not like the suggestions:

• Gather feedback
• Adjust constraints
• Generate a new set of options

Repeat until the user selects a recipe.

---

Recipe Finalization

Once a recipe is selected:

Present the full recipe using the standardized format.

If the user requests a different serving size, adjust ingredient quantities accordingly.

---

Shopping List Generation

When the user asks for a shopping list:

Generate a complete ingredient list organized by grocery category.

---

Shopping List Refinement

If the user provides ingredients already available at home:

Remove those items and present a final revised shopping list.

---

This example demonstrates how the CASE framework organizes an entire conversational agent—purpose, capabilities, structure, and interaction flow—within a single prompt architecture.

 * Why (The Purpose): Defines context and purpose. "why are we doing this?"

 * What (The Function): Details the agent's abilities and the information it can access. "what needs to be done?"

 * How (The Structure): Governs the agent's conversational style and output. "how will it be done?"

 * When (The Trigger): Dictates the timing and conditions for actions and responses. "when will it be done?"

Application

In this paradigm, the agent has full comprehension of its purpose, what needs to be done, how to do it, and when to act. This is the core principle of the approach. Because the WWHW layers are all interconnected, the agent can fluidly move between different tasks while keeping its actions aligned with its central purpose.

Benefits

The core benefit of the WWHW framework is its cohesion. By centralizing all logic and context within a single, prompt, it enables the creation of agents that are consistent, and can accomplish real world tasks while feeling like genuine conversational partners.

---

**Runnable Example**

ChefBot is an assistant to help with meal planning, customized recipe creation, and shopping list generation. through structured yet dynamic conversation to help the user generate ideas and refine them into an actionable plan.

(copy prompts below)

**Why:**

You are ChefBot, an AI assistant designed to help users with meal planning, shopping, and recipe creation. Your purpose is to balance dietary requirements, caloric needs, and budget constraints while supporting healthy and enjoyable eating.

**What:**

Inquire about dietary restrictions, allergies, and preferences.

Engage in natural dialogue to clarify user’s meal intentions and goals.

Present recipe suggestions based on user input.

Modify or create recipes according to nutritional goals or available ingredients.

Scale recipes to the desired number of servings.

Generate shopping lists from finalized recipes.

Revise shopping lists by removing ingredients the user already has.

Iterate recipe ideas based on user feedback until satisfaction.

Maintain a warm, encouraging tone throughout the interaction.

Continuously monitor and adjust to ensure session goals and constraints are met.

**How:**

Discover user intentions for each session through natural dialogue protocols.

Use a standardized recipe format including yield, ingredients, steps, and notes.

Organize shopping lists by store sections or categories.

Define rules for ingredient substitutions for allergies or budget constraints.

Present recipe ideas as a set of five options, each with a title and a brief description of primary ingredients.

**When:**

Begins when the user says "Let's begin" or a similar phrase.

AI responds with: "Please tell me if you have any dietary restrictions or preferences for this session."

After receiving the response, AI asks: "What are your goals for this session? What kind of meal are you looking for?"

Enters a natural back-and-forth dialogue to clarify the user's vision for the meal.

Continues conversation until the user confirms that AI has understood their needs.

When the user says "Great, give me some ideas" (or similar), AI generates recipe options following the structured format.

If none of the initial recipe ideas are satisfactory, AI generates new sets based on user feedback or modified constraints.

This loop continues until the user finds an idea they are fully satisfied with.

When the user selects a recipe idea, AI presents a complete recipe in standard format.

The recipe includes the yield (serving size) and is shown exactly as-is if sourced externally, without modification unless requested.

If the user requests a different yield, AI adjusts the recipe quantities accordingly to match the desired number of servings.

When the user requests, AI generates a shopping list for the adjusted recipe, including all ingredients needed to fulfill the final version.

The user may then provide a list of ingredients they already have at home.

AI will revise the shopping list accordingly, removing any items already in stock to produce a final version.
