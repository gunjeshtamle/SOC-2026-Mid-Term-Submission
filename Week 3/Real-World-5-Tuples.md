# Real World 5-Tuples
## Home Theromstat
***How it works:*** Decides when to heat or cool a room  
***States(S):*** Cold (<18°C), Comfortable (18–22°C), Hot (>22°C)  
***Actions(A):*** Heat On, Cool On, Do Nothing  
***Transitions(T):*** Heat on: Cold -> Comfortable (0.8), Cold -> Cold (0.2); Cool on: Hot -> Comfortable (0.8), Hot -> Hot (0.2); Do Nothing: Comfortable -> Comfortable (0.8), Comfortable -> Cold (0.2)  
***Rewards(R):*** Being in comfortable - +10, Being in Hot or Cold - -5, Per step heat or cool is on - -1  
***Discount(γ):*** 0.95, values long term comfortability as well as energy effeciency
## Inventory Restocking
***How it works:*** Measures current stock  
***States:*** 0 (stockout), 1–4 (low), 5–7 (healthy), 8–10 (overstocked)  
***Actions:*** Order 0, Order 3, Order 6, Order 9  
***Transitions:*** Next stock = current stock + ordered − daily demand. Daily demand: 0 units with prob. 0.1, 1 with 0.4, 2 with 0.3, 3 with 0.2. Demand in excess of stock is simply lost (no backorders). Stock cap = 10 (warehouse limit). 
***Rewards:*** unit sold (+5), stockout (-10), per unit held overnight - storage cost (-0.5), per order placed - fixed ordering cost (-2) 
***Discount:*** 0.95, values long term profit
