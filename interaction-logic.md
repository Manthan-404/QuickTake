# Interaction Logic: The Generative UI Lifecycle

QuickTake replaces the standard chatbot "loop" with a **Product-Driven Synthesis** flow.

### Phase 1: Product Recognition & Autonomous Start
The interaction begins with a product name. The system bypasses the "How can I help you?" stage and moves straight to **Heuristic Reasoning**. The UI renders a "Reasoning Trace" followed by the Compressed Explanation.

### Phase 2: Category-Based Weighting
The engine weights the response based on the category of the product identified. 
* *Example:* If the product is a "Diet Soda," the engine ignores calorie count and automatically weights the "Artificial Sweetener" and "Metabolic Signaling" lens as the priority.

### Phase 3: Non-Linear UI Mutation
Traditional logic restarts a conversation when parameters change. QuickTake **mutates** the existing UI. 
* If a user adds a lens (e.g., "Is this okay for kids?"), the system updates the **Tradeoff** and **Quick Take** sections within the existing UI component while maintaining the original product context in the background. This reduces visual clutter and keeps the focus on the evolving decision.
