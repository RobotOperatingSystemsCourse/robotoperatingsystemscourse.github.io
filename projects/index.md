---
title: Projects
layout: page
nav_order: 5
has_children: true
has_toc: false
---

# Projects
There are 6 projects in this course. Each project will be released after a lecture session and will be due immediately before another lecture section.

This course will use the [EECS Autograder](https://autograder.io) for submitting and grading course projects.

Projects are each worth 10 points and are composed of features, which are assigned point values based on difficulty and relevance to course learning objectives. Each feature will have several public and private tests on the autograder. In order to receive points for a project feature, it must pass all of its corresponding tests in the autograder. Each student will have 2 submissions per day for projects.

For example:

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Failed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Passed

This submission would receive a score of 5/10 because Feature A is incomplete.

## Late Policy
The late policy applies at the feature level of the projects. If a project is submitted after the deadline, only the features that have been updated since the previous submission are subject to the late policy.

- 100%: feature completed on time
- 80%: feature completed before next project deadline
- 60%: feature completed before 2 project deadlines out
- 50%: feature completed before final grading deadline

For example, if this submission occurred after the deadline (but before the next project's deadline) with no previous successful submissions:

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Failed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Passed

The student would receive 4/10 points. If the student then submitted again, completing all features:

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Passed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Passed

They would receive 8/10 points.

**Warning!** If a submission after the deadline breaks a working feature, that feature is now subject to the late policy. For example, if a student makes the following submission on time:

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Failed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Passed

Their score would be 5/10 points. If they were to submit again, after the deadline, to attempt to get the 5 points for Feature A, and in doing so broke Feature B, then Feature B would now be subject to the late policy.

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Passed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Failed

Their score would now be 4/10, and with a final submission that fixes Feature B:

### Test Project
1. Feature A (5 Points)
- Test 1: Passed
- Test 2: Passed
2. Feature B (5 points)
- Test 1: Passed
- Test 2: Passed

The student would receive a final project grade of 8/10.