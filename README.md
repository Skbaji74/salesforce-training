mkdir -p salesforce-training
cd salesforce-training
git init

cat << 'EOF' > README.md
# Salesforce Training Repository

## Overview
This repository contains daily coursework, code snippets, and output logs from the Salesforce Training program. 

## Structure
* **Weeks:** Organized chronologically (e.g., `week1`, `week2`).
* **Days:** Daily subdirectories (e.g., `day1`, `day2`).
* **Contents:** Each daily folder contains a dedicated `README.md`, working code files, and output logs.

## Quick Navigation
* [Week 1, Day 1](./week1/day1/)
* [Week 1, Day 2](./week1/day2/)
* [Week 1, Day 3](./week1/day3/)
* [Week 1, Day 4](./week1/day4/)
* [Week 1, Day 5](./week1/day5/)
EOF

for i in {1..5}; do
  mkdir -p "week1/day$i"
  touch "week1/day$i/daily_code.apex" "week1/day$i/output.txt"
  
  cat << EOF > "week1/day$i/README.md"
# Week 1 - Day $i

## Topics Covered
* [Insert Topic 1]
* [Insert Topic 2]

## Tasks Completed
1. [Insert Task 1]
2. [Insert Task 2]

## Code Files
* \`daily_code.apex\`: Implementation scripts.
* \`output.txt\`: Execution logs and results.

## Key Takeaways
* [Insert Notes]
EOF
done

echo "Repository 'salesforce-training' initialized successfully."

