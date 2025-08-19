# mean-variance-std-calculator
# main.py
from mean_var_std import calculate

def main():
    # Example test case
    print("Test with [0,1,2,3,4,5,6,7,8]:")
    print(calculate([0,1,2,3,4,5,6,7,8]))

    # Another test case
    print("\nTest with [9,8,7,6,5,4,3,2,1]:")
    print(calculate([9,8,7,6,5,4,3,2,1]))

    # Invalid test case (should raise ValueError)
    try:
        print("\nTest with [1,2,3]:")
        print(calculate([1,2,3]))
    except ValueError as e:
        print("Error:", e)

if __name__ == "__main__":
    main()
