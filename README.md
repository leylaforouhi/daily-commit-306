def calculate_bmi(weight, height):
    if weight <= 0 or height <= 0:
        raise ValueError("Weight and height must be positive")

    return weight / (height ** 2)


if __name__ == "__main__":
    weight = 72
    height = 1.78

    bmi = calculate_bmi(weight, height)

    print(f"Weight: {weight} kg")
    print(f"Height: {height} m")
    print(f"BMI: {bmi:.2f}")
