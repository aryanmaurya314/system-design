> _Before discussing the architecture, I’d like to clarify the requirements so we’re aligned on the scope. I’ll split them into functional and non-functional requirements._ 

## Ride Sharing App: like Uber/Ola/Rapido

### Functional Requirements
- Only authenticated users can book a ride
- Users can select source, destination and type of vehicle
- System will be able to find nearby available vehicles  matched with user's request
- User will receive an OTP after driver accepts the request
- Ride must not start before OTP verification
- User and driver both can see route in real time
- Once ride is completed billing will calculated 
- User should have option to pay in cash, upi, or card
- Once payment confirmed both driver and user should have option to rate themselves
### Non Functional Requirements
- High Availabilty: System must be available for accepting ride booking and tracking
- Scalability: Our system can handle thousands of current ride booking and route tracking at a time


