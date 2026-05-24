# PID and Lag-Lead Controller Design

## Overview

This project focuses on classical control system design using root locus analysis, transfer function modeling, MATLAB verification, and Simulink/Simscape implementation concepts.

The project includes PID controller design for a third-order unity feedback plant and lag-lead compensator design for a type 1 feedback control system. The goal was to compare hand calculations with MATLAB and Simulink verification results.

**Project Report:** [View PDF](pid-lag-lead-controller-final-report.pdf)  
**MATLAB Verification:** [View PDF](pid-lag-lead-matlab-verification.pdf)

## Key Skills

Control Systems, PID Control, Lag-Lead Compensation, Root Locus, Transfer Functions, MATLAB, Simulink, Step Response Analysis, Steady-State Error, Error Analysis

## Project Highlights

- Designed and tuned PID and lag-lead controllers using root locus analysis and transfer function modeling.
- Verified controller performance in MATLAB and Simulink.
- Compared uncompensated, PD, PID, and lag-lead step responses.
- Evaluated system performance using overshoot, peak time, settling time, rise time, and steady-state error.
- Documented error analysis between hand calculations and simulation results.

## PID Controller Design

The PID controller was designed to target 15% overshoot, reduced peak time, and zero step steady-state error.

Final PID gains:

- Kp = 253.69
- Ki = 125.25
- Kd = 6.400

## Lag-Lead Compensator Design

A lag-lead compensator was designed for a type 1 control system to improve transient response and reduce ramp steady-state error.

The design targeted:

- 50% reduction in settling time
- 90% reduction in ramp steady-state error

## Resume Bullets

- Designed and tuned PID and lag-lead controllers using root locus analysis, transfer function modeling, and MATLAB/Simulink verification.
- Compared uncompensated, PD, PID, and lag-lead step responses to evaluate overshoot, peak time, settling time, and steady-state error.
