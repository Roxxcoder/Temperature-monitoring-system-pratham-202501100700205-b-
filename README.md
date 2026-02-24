# Temperature-monitoring-system-pratham-202501100700205-b-
import random
import time

min_temp = float(input("Enter minimum temperature limit: "))
max_temp = float(input("Enter maximum temperature limit: "))

print("\nTemperature Monitoring Started...\n")

while True:
    current_temp = random.uniform(min_temp - 10, max_temp + 10)
    current_temp = round(current_temp, 2)
    
    print("Current Temperature:", current_temp, "°C")
    
    if current_temp < min_temp:
        print("Status: Temperature is LOW\n")
    elif current_temp > max_temp:
        print("Status: Temperature is HIGH\n")
    else:
        print("Status: Temperature is NORMAL\n")
    
    time.sleep(2)
