```
import traceback

def debug_data_code(data_code):
    try:
        # Execute the provided data code
        exec(data_code)
        print("Code executed successfully!")

    except Exception as e:
        print(f"Error: {str(e)}")
        print("Traceback:")
        traceback.print_exc()

if __name__ == "__main__":
    # Example data code (replace this with your actual data code)
    example_data_code = """
    data = [1, 2, 3, 4]
    result = sum(data) / 0  # This will cause a division by zero error
    print(result)
    """

    # Call the debugging service with the example data code
    debug_data_code(example_data_code)
```



