# Real World 5-Tuples
## Home Theromstat
***How it works:*** Decides when to heat or cool a room  
***States(S):*** Cold (<18°C), Comfortable (18–22°C), Hot (>22°C)  
***Actions(A):*** Heat On, Cool On, Do Nothing  
***Transitions(T):*** Heat on: Cold -> Comfortable (0.8), Cold -> Cold (0.2); Cool on: Hot -> Comfortable (0.8), Hot -> Hot (0.2); Do Nothing: Comfortable -> Comfortable (0.8), Comfortable -> Cold (0.2)  
***Rewards(R):*** Being in comfortable - +10, Being in Hot or Cold - -5, Per step heat or cool is on - -1  
***Discount(γ):*** 0.95, values long term comfortability as well as energy effeciency
