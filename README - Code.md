# Smart Grocery Chat Assistant using Model Context Protocol (MCP)

This project is a **context-aware chat assistant** that helps users plan meals and generate personalized grocery lists. Built using the **Model Context Protocol (MCP)**, the assistant tailors its responses based on:

-This simulates MCP with simple logic and mimics a chat assistant:
# Smart Grocery Assistant using Model Context Protocol (MCP)
print("Welcome to Smart Grocery Assistant!")

# Simulated MCP context
context = {
    "user": "Jane",
    "environment": "Mobile in Kitchen",
    "time": "Sunday 6 PM",
    "intent": "Plan healthy meals and shop under $100",
    "diet": "Low carb, kid-friendly",
    "history": ["Pasta", "Tacos", "Grilled Chicken"]
}

# Assistant response based on context
def meal_planner(context):
    print("\n--- CONTEXT RECEIVED ---")
    for k, v in context.items():
        print(f"{k.capitalize()}: {v}")
    
    print("\nBased on your preferences, here's your weekly plan:")
    
    meals = ["Veggie Stir Fry", "Chicken Salad", "Turkey Chili"]
    groceries = ["Chicken", "Broccoli", "Lettuce", "Beans", "Bell Peppers", "Olive Oil"]
    
    # Personalization based on history
    if "Turkey Chili" in context['history']:
        meals[2] = "Mac & Cheese with Hidden Veggies"
        groceries.remove("Beans")
        groceries.append("Pasta, Cheese, Carrots")
        print("\nNote: Replaced Turkey Chili since it was in your history.")
    
    print("\nMeals:")
    for meal in meals:
        print(f"- {meal}")
    
    print("\nGroceries:")
    for item in groceries:
        print(f"- {item}")

meal_planner(context)

---

### Creator
Sai Sravan Cherukuri 
Contact: www.linkedin.com/in/sai-sravan-cherukuri-irs
https://www.saisravancherukuri.com/

