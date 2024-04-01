# Quiz051

## 1. Solution
```.py
class Aircraft:
    def __init__(self, model: str, capacity: int):
        self.model = model
        self.capacity = capacity

    def get_info(self):
        return f"{self.model} (Capacity: {self.capacity})"


class Flight(Aircraft):
    def __init__(self, flight_number: str, origin: str, destination: str, departure_time: str, duration: list[int],
                 model: str, capacity: int):
        super().__init__(model, capacity)
        self.flight_number = flight_number
        self.origin = origin
        self.destination = destination
        self.departure_time = departure_time
        self.duration = duration

    def get_duration(self):
        return f"{self.duration[0]} hours {self.duration[1]} minutes and {self.duration[2]} seconds"

    def get_info(self):
        return f"""Flight {self.flight_number} from {self.origin} to {self.destination} departs at {self.departure_time} 
and lasts {self.get_duration()}. Aircraft: {super().get_info()}"""


def print_object_info(object):
    print(object.get_info())


aircraft = Aircraft(model="Boeing 737", capacity=150)
flight = Flight(flight_number="AA123", origin="New York", destination="Los Angeles", departure_time="10:00 AM",
                duration=[5, 30, 3], model="Boeing 737", capacity=150)

print_object_info(aircraft)
print_object_info(flight)

```
## 2. Proof of Work
![Quiz051](https://github.com/AntGra25/unit4-CS24/assets/142757981/728855ef-6941-4875-a403-fa59e5f0f28c)


## 3. UML Diagram

![Quiz051C](https://github.com/AntGra25/unit4-CS24/assets/142757981/f89a2bd0-121f-47df-aa84-ea99c59bfbda)


