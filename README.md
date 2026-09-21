def calculate_simple_interest(principal, rate, time):
    """
    Calculates simple interest.
    Principal: Initial amount
    Rate: Annual interest rate (in percentage)
    Time: Time period in years
    """
    interest = (principal * rate * time) / 100
    total_amount = principal + interest
    return interest, total_amount

# Example usage:
if __name__ == "__main__":
    P = float(input("Enter principal amount: "))
    R = float(input("Enter annual interest rate (%): "))
    T = float(input("Enter time period (years): "))
    
    interest, total = calculate_simple_interest(P, R, T)
    print(f"Simple Interest: {interest}")
    print(f"Total Amount: {total}")
