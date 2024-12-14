# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array. The bug is an infinite loop caused by improper use of the dependency array. 

## Bug Description
The `useEffect` hook is used to perform side effects in functional components.  However, if the dependencies array is missing or incorrect, this can lead to unexpected behavior, most notably an infinite render loop. 

## How to Reproduce
Clone the repository and run the app. You will observe the console logging rapidly due to the infinite loop. This is because the effect is constantly re-running. 

## Solution
The solution involves adding `count` to the dependency array of the `useEffect` hook. By doing so, the effect only runs when the `count` variable changes.