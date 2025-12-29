# QuickTake Reasoning Workflow

### Step 1: Input Detection
* Receive user input (String).
* **Determine Input Type**:
    * **IF** input matches a product pattern -> **Mode: Product Retrieval**
    * **ELSE** -> **Mode: Ingredient Parsing**

### Step 2: Profile Extraction
* **If Mode: Product Retrieval**: Fetch profile from knowledge base (e.g., "Tropicana Orange Juice" -> High Sugar, Vitamin C).
* **If Mode: Ingredient Parsing**: Scan text for "Signature Markers" (e.g., "Carrageenan" -> Digestive Irritant).

### Step 3: Intent Inference (Sense-Making)
* **Assign** a dominant reasoning lens based on the category or the highest-weight ingredient.
* *Example*: If a list contains 5+ stabilizers, the system defaults to a "Processing Lens" even if macros are "clean."

### Step 4: Synthesis (Decision Compression)
* Generate the **Quick Take** conclusion.
* Define the **Pivot** (The "Why").
* Identify the **Tradeoff** and **Uncertainty**.

### Step 5: UI State Management
* **Check**: Is the UI already active?
* **If YES**: Mutate the existing fields (Transition from old reasoning to new).
* **If NO**: Render a new specialized QuickTake payload.

### Step 6: Lens Refinement
* Wait for optional user context (e.g., "Low Sodium").
* **Loop to Step 3**: Re-reason the *same data* (Name or List) through the new lens and update the UI.
