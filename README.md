# HERMES Agent

![Hermes Logo](assets/hermes_logo.png)

Azim Ospanov <sup>1</sup>, Farzan Farnia <sup>2</sup>, Jiacheng Sun <sup>1</sup>, Haoli Bai <sup>1</sup>, Xin Shen <sup>3</sup>, Zijin Feng <sup>2</sup>


<sup>1</sup> <sub>**Noah's Ark Lab** ; </sub> <sup>2</sup> <sub>**The Chinese University of Hong Kong** ; </sub> <sup>3</sup> <sub>**Celia Team**</sub>

## Overview 
This repository accompanies ["HERMES: Towards Efficient and Verifiable Mathematical Reasoning in LLMs"]() work published on Arxiv. The codebase contains the agent implemented with LangChain and additional documentation on how to set it up with Lean4. The high-level overview of the method is below:

![Hermes Overview](assets/hermes_overview.png)


## Evaluation Results

<table>
  <tr>
    <th></th>
    <th colspan="4">Qwen3-8B</th>
    <th colspan="4">OpenAI o3-mini</th>
    <th colspan="4">DeepSeek-V3.1</th>
  </tr>
  <tr>
    <td></td>
    <td>MATH</td>
    <td>AIME</td>
    <td>CM</td>
    <td>HM2</td>
    <td>MATH</td>
    <td>AIME</td>
    <td>CM</td>
    <td>HM2</td>
    <td>MATH</td>
    <td>AIME</td>
    <td>CM</td>
    <td>HM2</td>
  </tr>
  <tr>
    <td>ZS-CoT@1</td>
    <td>84.8</td><td>20.0</td><td>69.1</td><td>4.3</td>
    <td>95.8</td><td>63.3</td><td>75.2</td><td>23.2</td>
    <td>94.8</td><td>46.7</td><td>78.0</td><td>22.7</td>
  </tr>
  <tr>
    <td> Majority@5 </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> Skywork </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> ArmoRM </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> Shepherd </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> RLHFLow </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <th colspan="13" align="left"><i>Lean-Based Methods</i></th>
  </tr>
  <tr>
    <td> Safe </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> Safe* </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
  <tr>
    <td> <i> <b>HERMES</b> </i> </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
    <td>  </td><td>  </td><td>  </td><td>  </td>
  </tr>
</table>


