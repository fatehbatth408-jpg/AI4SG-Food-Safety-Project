# AI4SG Food Safety Project

## Problem

Every day, a lot of food banks and donation places get food that is broken or out of date. A lot of the time, volunteers have to quickly decide if food is safe, not safe, or needs more testing. This is hard to do when there are a lot of gifts but not enough trained workers.

Our project's main goal is to make it easier for food bank workers in San Jose to find donated food that might not be safe faster. Maria is a specific user. She is a volunteer who sorts given food during times when there are a lot of donations. At the moment, the failure point is when helpers are too busy or don't know what to do and miss damaged cans or expired goods.


## AI Capability

The Gemini API is used for image recognition and organized data extraction in our project. These AI skills are useful for the job because they let the system look at pictures of food items that people share and find damage, concerns about when they will go bad, and safety risks.

We used the same AI skills that we worked on in Labs 2 and 3. What the AI does is help organize written and visual information into safety tips that workers can quickly understand.


## Workflow

1. A volunteer uploads a photo of donated food.
2. The Gemini AI analyzes the image.
3. The system identifies:
   - food item
   - package condition
   - expiration concern
   - risk level
   - recommended action
4. The AI returns a structured response.
5. The volunteer reviews the output and decides whether to keep, inspect, or discard the item.

### Example Output
- Food Item: Canned Beans
- Package Condition: Dented
- Risk Level: Medium
- Recommended Action: Manual Inspection Required

The system helps volunteers process donations faster while reducing unsafe food distribution.

## Failure Case

In one case, the AI looked at a picture of a dented can but couldn't fully tell if the can was actually dangerous or just badly damaged. The AI gave the item a "medium risk" rating, even though some broken cans may pose major contamination risks.

This showed that image recognition can have trouble with cases that are close to being perfect or pictures that aren't clear. A volunteer who only relies on the AI could accept food that isn't safe by accident.

## Oversight and Tradeoff

Before any food is allowed to be distributed, it should be looked over by people. The AI should help workers, not take their place.

We agreed that all high-risk and medium-risk items should have to be inspected by hand. This makes it less likely that food that isn't safe will be given out, but it takes longer to sort and needs more worker time.

## Screenshots

### Gemini API Setup
<img width="1901" height="384" alt="Screenshot 2026-05-22 at 12 36 28 AM" src="https://github.com/user-attachments/assets/56b9c116-22fa-47a4-90a8-46683d644cc1" />

### Structured AI Output
<img width="1883" height="1046" alt="Screenshot 2026-05-22 at 12 37 58 AM" src="https://github.com/user-attachments/assets/2f395a14-1327-454f-9a6f-6b01fef3d897" />

### Food Safety Image Analysis
<img width="1831" height="955" alt="Screenshot 2026-05-22 at 12 39 36 AM" src="https://github.com/user-attachments/assets/7b2778be-471b-43cb-a057-eb5126face11" />
