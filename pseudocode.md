# QuickTake Reasoning Workflow

### Step 1: Input Capture
* Receive **Product Name** from user.
* Check for any active "User Lenses" (e.g., Keto, Vegan, Gut Health).

### Step 2: Product Profile Retrieval
* Match the input name against the internal knowledge base.
* Identify "Signature Markers" (e.g., specific sweeteners, protein sources, or degree of processing).

### Step 3: Intent Inference (Sense-Making)
* Identify the product's primary category.
* **Assign** a dominant reasoning lens based on that category.
* *Logic*: If the product is a "Breakfast Cereal," the system defaults to the "Sugar/Satiety" lens as the primary weight.

### Step 4: Synthesis (Decision Compression)
* Generate the **Quick Take** (The bottom-line conclusion).
* Define the **Pivot** (The core "Why").
* Identify the **Tradeoff** (The necessary nuance).
* Identify the **Uncertainty** (The gray area).

### Step 5: UI State Management
* **Check**: Is there an existing UI component visible?
* **If YES**: Mutate the specific fields within that component with a smooth transition.
* **If NO**: Render a new specialized QuickTake UI payload.

### Step 6: Context Injection
* If the user adds a specific goal (e.g., "I have high blood pressure"):
* **Loop back to Step 3** to re-calculate weights.
* Update the existing UI with the new reasoning without losing the product profile.
