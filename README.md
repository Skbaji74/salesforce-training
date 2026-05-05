# salesforce-training

## Overview
This repository contains all my daily coursework, code snippets, and output files from the Salesforce Training program. 

## Structure
The repository is organized chronologically to easily track progress:
* **Weeks:** Separated into `week1`, `week2`, etc.
* **Days:** Inside each week, the work is divided into `day1`, `day2`, etc.
* **Daily Contents:** Each daily folder contains:
  * A dedicated `README.md` summarizing the day's topics.
  * Source code files.
  * Output files and execution logs.

## Quick Navigation
* [Week 1, Day 1](./week1/day1/)
* [Week 1, Day 2](./week1/day2/)
* [Week 1, Day 3](./week1/day3/)
* [Week 1, Day 4](./week1/day4/)
* [Week 1, Day 5](./week1/day5/)
EOF

# 4. Create Week 1 structure and daily files
for i in {1..5}
do
  # Create the day folder
  mkdir -p "week1/day$i"
  
  # Create the blank code and output files
  touch "week1/day$i/daily_code.apex"
  touch "week1/day$i/output.txt"
  
  # Create and populate the daily README.md
  cat << EOF > "week1/day$i/README.md"
# Week 1 - Day $i

## Topics Covered Today
* (topic here)

## Tasks Completed
1. 
2. 

## Code Files
* \`daily_code.apex\`: Contains the scripts written during today's session.
* \`output.txt\`: Contains the console execution results.


