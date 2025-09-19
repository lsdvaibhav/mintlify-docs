# Jewellery Ad Workflow in ElseIf.ai

## Objective

Build a **workflow in ElseIf.ai** that allows a jewellery business user to upload:

1. A few **ornament images** (necklace, bracelet, rings, etc.)
2. A **model image**

→ and automatically generate a **no-voice, professional ad video** showcasing the jewellery on the model.

The workflow must use **Gemini Nano Banana** as the LLM backbone for orchestration.

---

## Requirements

### 1. Inputs (Business User View)
- Ornament image(s)  
- Model image  
- Optional: brand name / tagline  

### 2. Workflow Steps (ElseIf.ai Implementation)

**Image Preprocessing**
- Remove any existing jewellery from model image.  
- Place uploaded jewellery onto the model (realistic fit).  

**Ad Video Creation**
- Use reference JSON prompt (Jewellery template from *AI Ads Mastry*).  
- Style: professional studio, cinematic lighting, 9:16 vertical ad format.  
- No voice, but include **text overlay option** (brand name / tagline).  

**Output**
- Generate a **short ad video (5–8 sec)** with smooth camera movement.  
- Export in **.mp4** format, ready for Instagram/TikTok.  

### 3. Test Cases (Candidate Must Handle)
- **Case 1**: One necklace + one model image → Ad video with necklace correctly placed.  
- **Case 2**: Multiple ornaments (e.g., ring + necklace) → Generate **two ad variants**, one per ornament.  
- **Case 3**: Text overlay enabled (brand tagline).  
- **Case 4**: Incorrect input (e.g., missing model image) → Workflow should return a **clear error message**.  

### 4. Tech Constraints
- Workflow must be built **entirely in ElseIf.ai**.  
- Must use **Gemini Nano Banana** as the reasoning engine for orchestration.  
- Outputs must be **deterministic JSON-driven video generation** (no manual editing).  

### 5. Deliverables
- ElseIf.ai workflow export (YAML/JSON).  
- Documentation: **Step-by-step guide** for a non-technical jewellery shop owner on how to use it.  
- Demo video samples for at least **2 test cases**.  

---

## Evaluation Criteria
- ✅ **Correctness** – Jewellery is realistically placed on model.  
- ✅ **Workflow Quality** – Uses Gemini Nano Banana effectively.  
- ✅ **Error Handling** – Workflow doesn’t break on bad inputs.  
- ✅ **Usability** – Easy for an end-business user.  
- ✅ **Documentation** – Simple instructions for jewellery shop owners.  
