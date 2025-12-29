# Interaction Logic: The Generative UI Lifecycle

QuickTake replaces the standard chatbot loop with a **Unified Synthesis** flow that handles multiple entry points.

### Phase 1: Input Bifurcation
The system identifies the input type without user prompts.
* **If Name**: The system fetches the product profile and identifies the category.
* **If Ingredients**: The system bypasses data-fetching and moves straight to **Heuristic Reasoning** on the provided text.
Both paths lead to a "Reasoning Trace" that shows the user how the system is thinking.

### Phase 2: Autonomous Weighting
The engine automatically selects the "Dominant Concern." 
* *Example:* For a "Diet Soda" or a list containing "Aspartame," the engine ignores calorie count and weights "Artificial Sweeteners" as the priority concern.

### Phase 3: Non-Linear UI Mutation
QuickTake **mutates** the existing UI rather than creating a new message thread.
* If a user changes the lens (e.g., from "General Health" to "Diabetes-Friendly"), the UI components update their values in real-time. The **Quick Take** and **Tradeoff** sections refresh to reflect the new priority while keeping the original product/ingredient context active in the background.
