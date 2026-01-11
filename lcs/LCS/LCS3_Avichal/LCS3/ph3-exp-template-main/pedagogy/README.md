#### Please use the [reference](https://github.com/virtual-labs/ph3-exp-dev-process/blob/main/pedagogy/README.org) document to fill this template.  Follow the [link](https://github.com/virtual-labs/ph3-exp-dev-process/tree/main/sample/pedagogy) to view a sample pedagogy document.

## Pedagogy
<p align="center">

<br>
<b> Experiment : Longest Common Subsequence (LCS) Visualizer <a name="top"></a> <br>
</p>

<b>Discipline | Computer Science & Engineering <b> 
:--|:--|
<b> Lab | Algorithms & Data Structures Lab <b> 
<b> Experiment| Longest Common Subsequence: Algorithm Visualization and Comparison <b> 


<h4> [1. Focus Area](#LO)
<h4> [2. Learning Objectives ](#LO)
<h4> [3. Instructional Strategy](#IS)
<h4> [4. Task & Assessment Questions](#AQ)
<h4> [5. Simulator Interactions](#SI)
<hr>

<a name="LO"></a>
#### 1. Focus Area : Reinforce theoretical concept.

#### 2. Learning Objectives and Cognitive Level

| Sr. No | Learning Objective | Cognitive Level | Action Verb |
|:---|:---|:---|:---|
| 1. | Understand the concept of subsequences and the Longest Common Subsequence (LCS) problem | **Understand** | Explain, Describe, Identify |
| 2. | Apply dynamic programming approach to solve LCS problems | **Apply** | Implement, Execute, Demonstrate |
| 3. | Analyze and compare time-space complexities of different LCS algorithms (Standard DP, Rolling Array, Hirschberg) | **Analyze** | Compare, Contrast, Differentiate |
| 4. | Trace the backtracking process to reconstruct the actual LCS from DP table | **Analyze** | Trace, Reconstruct, Follow |
| 5. | Evaluate algorithm performance based on input characteristics | **Evaluate** | Judge, Assess, Recommend |

<br/>
<div align="right">
    <b><a href="#top">↥ back to top</a></b>
</div>
<br/>
<hr>

<a name="IS"></a>
#### 3. Instructional Strategy
###### Name of Instructional Strategy  :    <u> **Interactive Simulation with Guided Discovery**   
###### Assessment Method: **Pre-test/Post-test + Formative Feedback in Simulation**

<u> <b>Description: </b>    </u>
<br>
    
The instructional strategy follows a **Constructivist** approach where learners actively build knowledge through interaction with the simulation. The strategy is implemented in four phases:

1. **Activation Phase (Pre-test)**: Assess prior knowledge about sequences, subsequences, and basic algorithm concepts through multiple-choice questions.

2. **Exploration Phase (Simulation)**: 
   - Provide interactive visualization of three LCS algorithms with step-by-step execution
   - Enable real-time character comparison with visual feedback
   - Offer immediate explanations for each algorithmic step
   - Include adaptive examples with preset sequences

3. **Application Phase (Tasks)**:
   - Guided tasks with increasing complexity
   - Comparative analysis of algorithm performance
   - Backtracking reconstruction exercises

4. **Evaluation Phase (Post-test)**: 
   - Assess conceptual understanding and application skills
   - Measure learning gains through comparative analysis with pre-test

**Scaffolding Elements**:
- Step-by-step execution control (Step/Auto-play)
- Visual cues (color coding, highlighting, animations)
- Context-sensitive explanations
- Adaptive speed control for cognitive processing

<br/>
<div align="right">
    <b><a href="#top">↥ back to top</a></b>
</div>
<br/>
<hr>

<a name="AQ"></a>
#### 4. Task & Assessment Questions:

| Sr. No | Learning Objective | Task to be performed by the student in the simulator | Assessment Questions as per LO & Task |
|:---|:---|:---|:---|
| 1. | Understand subsequence and LCS concepts | Enter two sequences and use presets to observe LCS variations | Q1. What is the LCS of "ABCBDAB" and "BDCABA"?<br>Q2. How does LCS differ from longest common substring? |
| 2. | Apply dynamic programming approach | Step through Standard DP algorithm for given sequences, observe table filling | Q3. What value would dp[3][4] have for sequences "ABCD" and "ACBAD"?<br>Q4. Explain the recurrence relation for dp[i][j] when characters match. |
| 3. | Compare algorithm complexities | Run same sequences through all three algorithms, compare memory usage displays | Q5. For sequences of length 100, what is space saving of Rolling Array vs Standard DP?<br>Q6. When would you recommend Hirschberg's algorithm? |
| 4. | Trace backtracking process | Use step mode during traceback phase, follow highlighted path | Q7. From the backtracking path, reconstruct the LCS for "AGGTAB" and "GXTXAYB"<br>Q8. What does a diagonal arrow indicate in backtracking? |
| 5. | Evaluate algorithm performance | Test algorithms with different sequence types (match-heavy, sparse, long) | Q9. Which algorithm performs best for DNA sequences (long with few matches)?<br>Q10. Justify algorithm choice for real-time sequence comparison. |

<div align="right">
    <b><a href="#top">↥ back to top</a></b>
</div>
<br/>
<hr>

<a name="SI"></a>

#### 5. Simulator Interactions:

| Sr.No | What Students will do? | What Simulator will do? | Purpose of the task |
|:---|:---|:---|:---|
| 1. | Enter two sequences in input fields or select presets | Display character boxes for both sequences with indices, initialize statistics panel | Activate prior knowledge, set context for comparison |
| 2. | Select algorithm type (Standard DP, Rolling Array, Hirschberg) | Update algorithm info panel, modify pseudocode display, adjust visualization layout | Develop understanding of algorithm variations and trade-offs |
| 3. | Click "Initialize" button | Generate DP table structure, reset all visual elements, prepare for stepwise execution | Understand initialization phase of dynamic programming |
| 4. | Click "Step" button repeatedly | Highlight compared characters, update DP table cell, show step explanation, increment progress counter | Follow algorithm execution at own pace, reinforce recurrence relation understanding |
| 5. | Adjust speed slider during Auto-play | Change animation speed, update visual feedback timing | Accommodate different learning speeds, allow repetition for complex steps |
| 6. | Observe character comparison area | Animate character highlight, show match/mismatch indicators, display comparison result | Visualize the core comparison operation, understand match detection |
| 7. | Watch DP table during traceback | Highlight backtracking path in yellow, animate movement through table | Understand how LCS is reconstructed from DP values |
| 8. | Compare statistics across algorithms | Display real-time space usage, step counts, time complexity indicators | Develop analytical skills for algorithm comparison |
| 9. | Hover over help icons | Show contextual tooltips explaining interface elements | Provide just-in-time support without cluttering interface |
| 10. | Click "Reset" and try new sequences | Clear all visualizations, return to initial state | Encourage experimentation, test understanding with varied inputs |

<div align="right">
    <b><a href="#top">↥ back to top</a></b>
</div>
<br/>
<hr>

## Cognitive Load Management

**Intrinsic Load Management**:
- Break complex algorithm into discrete steps
- Provide visual separation between comparison phase and table update
- Use color coding consistently (blue for current, green for match, yellow for trace)

**Extraneous Load Reduction**:
- Minimalist interface with progressive disclosure
- Context-sensitive help
- Clear visual hierarchy (Input → Process → Output)

**Germane Load Enhancement**:
- Multiple representation (pseudocode + visualization + explanation)
- Interactive controls for self-paced learning
- Immediate feedback on actions

## Accessibility Features

1. **Keyboard Navigation**: All controls accessible via keyboard shortcuts
2. **Color-Blind Friendly**: Use patterns and icons in addition to colors
3. **Responsive Design**: Works on different screen sizes
4. **Clear Typography**: Readable fonts with sufficient contrast

## Learning Analytics Integration Points

The simulation tracks:
- Time spent on each algorithm
- Number of step executions
- Reset frequency (indicating exploration)
- Preset usage patterns
- Speed preference settings

These can be used for adaptive learning pathways in future enhancements.