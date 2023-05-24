# Minitalk Tester

The Minitalk Tester is a Python script designed to test the functionality of the Minitalk project from the 42 school. It automates the process of running various test cases to ensure that the server and client programs function correctly.

## Features

- Test basic functionality with different input strings
- Test the ability to handle large input strings
- Stress test the server-client exchange with multiple iterations
- Test bonus functionality with Unicode characters

## Prerequisites

Before using the Minitalk Tester, make sure you have the following:

- The Minitalk server program compiled and ready to run
- The Minitalk client program compiled and ready to run
- Python 3 installed on your system

## Usage

1. Clone the Minitalk Tester repository to your Minitalk folder.
2. Compile the Minitalk server and client programs.
4. If needed, modify the `PATH_TO_CLIENT` and `PATH_TO_CLIENT_BONUS` variables in the script to point to the compiled client programs.
5. Open a terminal and navigate to the directory where the Minitalk Tester script is located.
6. Run the following command to install the required dependencies:

```shell
	pip install psutil click termcolor
```

7. Run the Minitalk Tester script using the following command:

```shell
	python minitalk_tester.py [options]
```

The available options are:
- `-h, --help`: Display the help message
- `-a, --test_all`: Run all tests
- `-m, --test_mandatory`: Run only the mandatory tests
- `-b, --test_bonus`: Run only the bonus tests
- `-t1, --test_1`: Run Test 1 (basic functionality with a 100 char)
- `-t2, --test_2`: Run Test 2 (behavior when an empty string is passed)
- `-t3, --test_3`: Run Test 3 (ability to handle a string of 20,000 char)
- `-t4, --test_4`: Run Test 4 (stress test with multiple iterations of a 3,000 char)
- `-t5, --test_5`: Run Test 5 (bonus functionality with 100 Unicode char)
- `-t6, --test_6`: Run Test 6 (stress test with multiple iterations of a 4,000 Unicode char)

8. The Minitalk Tester will execute the selected tests and display the results in the terminal.

## Expected Output on the Server

- Test 1: The server should receive a string of 100 characters 'A' from the client.
- Test 2: The server should receive an empty string from the client.
- Test 3: The server should receive a string of 20,000 characters 'Y' from the client.
- Test 4: The server should receive multiple iterations of a string of 3,000 characters from the client. ('a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', j' 'k', 'l' 'm', 'o')
- Test 5: The server should receive a string of 100 Unicode characters 🦊 from the client.
- Test 6: The server should receive multiple iterations of a string of 4,000 Unicode characters from the client. ('🌑', '🌒', '🌓', '🌔', '🌕', '🌖', '🌗', '🌘', '🌙', '🌚')

Make sure to compare the actual output on the server with the expected output to verify the correctness of the Minitalk implementation.

## Important Note

- Ensure that the Minitalk server program is compiled and running

 before running the Minitalk Tester.
- Make sure to modify the `PATH_TO_CLIENT` and `PATH_TO_CLIENT_BONUS` variables in the script to point to the correct client programs.
- The Minitalk Tester script assumes that the server program is named "server" and the bonus server program is named "server_bonus". Modify the `SERVER_NAME` and `SERVER_NAME_BONUS` variables if your server programs have different names.

## Troubleshooting

If you encounter any issues while running the tester, please check the following:

- Make sure you have correctly installed and compiled the Minitalk server and client programs.
- Ensure that the server is running before you execute the tester.

## Contributing

Contributions to the Minitalk tester are always welcome! To contribute:

1. Fork this repository.
2. Create a new branch for your changes.
3. Submit a pull request with your changes.

Thank you for considering to contribute to the Minitalk tester!

Feel free to contact me.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
