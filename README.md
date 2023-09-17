- 👋 Hi, I’m @Allisnotavailable
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
-- Create a new car
local car = Instance.new("Model")
car.Name = "Car"
car.Parent = game.Workspace

-- Create the car body
local body = Instance.new("Part")
body.Size = Vector3.new(5, 1, 10)
body.BrickColor = BrickColor.new("Bright red")
body.Anchored = false
body.Parent = car

-- Create the wheels
local wheel1 = Instance.new("Part")
wheel1.Size = Vector3.new(2, 2, 2)
wheel1.BrickColor = BrickColor.new("Black")
wheel1.Anchored = false
wheel1.Parent = car

local wheel2 = wheel1:Clone()
wheel2.Parent = car

local wheel3 = wheel1:Clone()
wheel3.Parent = car

local wheel4 = wheel1:Clone()
wheel4.Parent = car

-- Set the wheel positions
wheel1.CFrame = body.CFrame * CFrame.new(2.5, -0.5, 5)
wheel2.CFrame = body.CFrame * CFrame.new(-2.5, -0.5, 5)
wheel3.CFrame = body.CFrame * CFrame.new(2.5, -0.5, -5)
wheel4.CFrame = body.CFrame * CFrame.new(-2.5, -0.5, -5)

-- Create Suspension Constraints
local suspension1 = Instance.new("HingeConstraint")
suspension1.Parent = car
suspension1.Attachment0 = body:FindFirstChild("Attachment")
suspension1.Attachment1 = wheel1:FindFirstChild("Attachment")

local suspension2 = suspension1:Clone()
suspension2.Parent = car
suspension2.Attachment0 = body:FindFirstChild("Attachment")
suspension2.Attachment1 = wheel2:FindFirstChild("Attachment")

local suspension3 = suspension1:Clone()
suspension3.Parent = car
suspension3.Attachment0 = body:FindFirstChild("Attachment")
suspension3.Attachment1 = wheel3:FindFirstChild("Attachment")

local suspension4 = suspension1:Clone()
suspension4.Parent = car
suspension4.Attachment0 = body:FindFirstChild("Attachment")
suspension4.Attachment1 = wheel4:FindFirstChild("Attachment")

-- Add mobile controls
local UserInputService = game:GetService("UserInputService")

local function moveCar(direction)
    -- Adjust car's position or rotation based on the mobile input
    -- You can implement the movement and rotation logic here
end

UserInputService.InputBegan:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.Touch then
        moveCar("forward") -- Adjust this based on your car's control logic
    end
end)

UserInputService.InputEnded:Connect(function(input)
    if input.UserInputType == Enum.UserInputType.Touch then
        moveCar("stop") -- Adjust this based on your car's control logic
    end
end)
--->
