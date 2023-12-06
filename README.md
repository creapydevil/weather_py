# weather_py
#Weather prediction program
def weather_prediction(t,H,w):
    W=0.5*t**2 - 0.2 *H + 0.1*w - 15
    return W
def predict_weather(W):
    if W >= 300:
        return "Sunny"
    elif 200 <= W < 300:
        return "Cloudy"
    elif 100<=W < 200:
        return "Rainy"
    else:
        return "Storms"

# Weather inputs
t = int(input())
H = int(input())
w = int(input())
# Calculations

weather_today=predict_weather(W)
# display weather today
print(f"predicted weather today: {weather_today}")
