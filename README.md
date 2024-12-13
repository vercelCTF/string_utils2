# string_utils2
def reverse_string(s):
    """
    Reverses the given string.
    """
    return s[::-1]

def is_palindrome(s):
    """
    Checks if the given string is a palindrome.
    """
    cleaned = ''.join(c.lower() for c in s if c.isalnum())
    return cleaned == cleaned[::-1]

if __name__ == "__main__":
    test_string = input("Enter a string: ")
    print(f"Reversed String: {reverse_string(test_string)}")
    print(f"Is Palindrome: {is_palindrome(test_string)}")
