# IS218 Test 1

Name: Bryan Asare

This project is my IS218 assessment covering Python project setup, addition and subtraction operations, automated testing, and project delivery.

The requirements.txt file is committed so everyone working on the project can install the same required Python packages. 
The .venv folder is ignored because it contains locally installed packages that can be recreated from requirements.txt.

Project Purpose

The purpose of this project was to learn how to set up a Python environment and use automated testing to make sure that the code works properly. For this assignment, I created two functions that perform addition and subtraction. I also used pytest to test both functions with different numbers to make sure they returned the correct answers.

Setting Up the Environment

One of the first things I had to do was set up my Python environment. I used Python 3.13.15 and created a virtual environment so that the packages needed for this project would be kept separate from the other Python installations on my computer.

These are the commands I used to set up my environment:

pyenv local 3.13.15
python3 -m venv .venv
source .venv/bin/activate

After creating the environment, I installed the packages listed in requirements.txt using:

python -m pip install -r requirements.txt

The requirements.txt file is committed to GitHub because it allows other people working on the project to install the same packages. The .venv folder, however, is ignored because it contains files and packages that can be recreated. Because of this, there is no reason to upload the entire folder to GitHub.

Running the Tests

Another important part of this assignment was learning how to use pytest. Instead of just assuming that the functions worked, I had to create tests that checked whether they returned the correct results.

To run the student tests, I used:

python -m pytest

To run both my tests and the acceptance tests provided by the professor, I used:

python -m pytest tests checks -v

After completing both functions, all 6 student tests and 6 acceptance tests passed.

Example of a Test

One test that I created was test_subtract_negative_result. For this test, I used the numbers 3 and 5 and expected the answer to be -2.

The purpose of this test was to make sure that the subtraction function could return a negative number instead of only positive numbers. The assertion checks whether the answer is equal to -2. If the function returns a different number, pytest will mark the test as failed.

One thing I learned from this assignment is that testing is useful because it helps identify mistakes that might not be noticeable just by looking at the code. This was something I experienced when I intentionally made my addition function return the wrong answer and pytest was able to catch it.

GitHub Issues

Throughout this assignment, I used GitHub issues to keep track of the different tasks that needed to be completed.

Issue #1: Setup

Issue #2: Addition

Issue #3: Subtraction

Issue #4: Delivery