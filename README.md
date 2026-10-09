# Pac-Man Search Algorithms

Shared baseline for the four-member search assignment. The `search/` directory contains the original, unmodified starter project from the supplied `search.zip`. Q1-Q7 implementations are intentionally left for the team to add on their own branches.

## Setup

Use Python 3.9-3.11, as required by the assignment. With Conda:

```sh
conda create -n cs188 python=3.11
conda activate cs188
pip install numpy matplotlib
cd search
python pacman.py
```

Check that the game opens and responds to the arrow keys.

## Team allocation

| Member | Questions | Suggested branch |
|---|---|---|
| 1 | Q1 DFS + Q5 CornersProblem | `feature/q1-q5-dfs-corners` |
| 2 | Q2 BFS + Q6 cornersHeuristic | `feature/q2-q6-bfs-heuristic` |
| 3 | Q3 UCS + Q4 A* | `feature/q3-q4-search` |
| 4 | Q7 foodHeuristic | `feature/q7-food-heuristic` |

Clone the repository and create your own branch from `main`:

```sh
git clone https://github.com/IT24102884/IA-Project-pacman-search-algorithms.git
cd IA-Project-pacman-search-algorithms
git switch -c YOUR_BRANCH_NAME
```

Replace `YOUR_BRANCH_NAME` with the assigned branch above. Review and apply only your assigned functions, test, commit your actual work, and open a pull request into `main`. Avoid replacing a whole shared file with an older copy. The separate handoff helper can target this repository's `search/` directory; handoff scripts and packages do not need to be added to the repository.

Q5's supplied grader needs Q2. Q6 needs Q5 and Q4. Q7 needs Q4. Members can work in parallel, but dependent tests require those implementations to be integrated. Everyone must understand the complete solution for the viva.

## Tests

Run inside `search/`:

```sh
python autograder.py -q q1
python autograder.py -q q2
python autograder.py -q q3
python autograder.py -q q4
python autograder.py -q q5
python autograder.py -q q6
python autograder.py -q q7
```

Add `--no-graphics` for a headless run. Tests are expected to fail while the starter functions remain unimplemented. Q8 is included in the original framework but is outside the assignment's Q1-Q7 scope.

## Assignment boundaries

- Implement Q1-Q4 in `search/search.py` and Q5-Q7 in `search/searchAgents.py`.
- Use the supplied `util.Stack`, `util.Queue` and `util.PriorityQueue` search containers.
- Preserve names, framework files, tests and original attribution notices.
- Keep real contribution records and declare AI assistance, including exact prompts, as required by the brief.
- Submit a standalone group report PDF and a separate ZIP containing only `search.py` and `searchAgents.py`. This repository is the development project, not that submission ZIP.

Use the supplied assignment brief as the marking authority. Its detailed scheme gives 40 marks for Q1-Q7, 10 for the report, 10 for individual Git work and 40 for the individual viva. The starter grader uses different point totals; do not edit it to match the PDF. Ask the lecturer to clarify the conflicting generic rubric on the brief's final page.

## Attribution and publication

The original Pac-Man framework and autograder were developed at UC Berkeley: http://ai.berkeley.edu. Original licensing and attribution notices remain in the starter files. The supplied brief requests a public repository, while the starter notices restrict publishing solutions; clarify the solution-publication requirement with the lecturer. This baseline contains no completed assignment solutions.
