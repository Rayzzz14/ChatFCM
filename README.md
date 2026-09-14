# ChatFCM
# ChatFCM

Official repository for our paper:

**ChatFCM: Comprehension-Synthesis Decoupling for LLM-Based Functional Coverage Model Generation**  
*ICCAD 2026*

## Overview

ChatFCM is an LLM-based framework for automatically generating **SystemVerilog functional coverage models** from hardware protocol specifications.

Unlike conventional end-to-end generation methods, ChatFCM decouples the task into two stages:

1. **Document Comprehension**  
   Extracts specification knowledge into a structured three-layer intermediate representation (IR), including:
   - Atomic entities
   - Derived entities
   - Relations

2. **Code Synthesis**  
   Generates sampling logic and covergroup constructs from the validated IR.

A derivation DAG is constructed to explicitly model dependencies between entities. DAG-based validation is further used to detect and repair extraction errors before code generation.

