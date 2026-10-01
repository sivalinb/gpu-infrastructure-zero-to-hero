# Fresh computer-science graduate persona review

**Review date: 2026-10-01. This is an AI-simulated learner perspective, not an independent human study or a measured learning-gain result.** The assumed learner can run beginner Python but has no prior expertise in this infrastructure domain.

## Does the beginning actually start at zero?

I start with serial and parallel work, CPU versus GPU, kernels, host RAM versus VRAM, and bytes versus GiB. Model parameters and precision come next. Request allowances, batching, training state, utilization, temperatures, clocks, error evidence, and placement then have a concrete foundation.

Every concept includes an analogy, worked example, misconception, glossary, practice explanation, and a four-state narrated animation. Play, Pause, Back, Next, pace, and the slider let me predict a change and inspect it. Reduced-motion handling and a readable state transcript provide another way to follow the explanation.

## Can I do more than remember names?

By the final levels I can explain every term in a capacity estimate, calculate integer batch limits, distinguish input starvation from thermal symptoms, preserve the meaning of gauge and counter fields, and check whole-GPU Pod requests. I can also explain why requesting two GPUs does not automatically partition a model or prove a speedup.

Five-question assessments require at least 80%, and a badge additionally requires the practical plan to pass two scenario variants. Later assessments unlock in order. Python recomputes practical results and owns the progress transaction; an AI answer or submitted success flag cannot award a badge. All lessons can still be previewed.

In the browser I entered the two batch calculations and observed a computed 23.04 GiB estimate within 24 GiB, with a contribution chart. At a 375-pixel viewport, animation cards stack vertically and the document has no horizontal overflow. The mobile screenshot is included in assets/mobile.jpg.

## Changes made after the review

The initial batch exercise could be passed by choosing a strategy. It now requires my calculated maximum batches for both 24 GiB and 20 GiB scenarios, independently regraded in Python. For the stated 7B FP16 weights, 2 GiB overhead, and 1 GiB/request assumptions, those answers are 8 and 4. This is a calculation check, with an explicit warning that a fit estimate is not a latency or OOM guarantee.

Shared improvements include retrieval of glossary terms and practice explanations, clearer quiz distractors, selected-topic tutor context, vertically stacked mobile animation scenes, and badge ordering that remains 0 through 10 on narrow screens. These changes address observed usability and reasoning gaps; they are not proof of human learning gains.

## What a badge establishes, and what remains

Passing establishes the included, bounded learning objectives and guided lab checks. Worked solutions and source code are available, attempts can be repeated, and these are not proctored exams. A badge alone cannot establish retention, independent diagnosis, or production expertise.

The default course uses transparent arithmetic and synthetic replay. It does not execute a CUDA kernel, measure a real model, run DCGM diagnostics, provision MIG, or deploy Kubernetes. Real workload output, memory, latency, collection health, and device-plugin scheduling must be verified on suitable hardware before independent operational claims.

The [independent capstone](INDEPENDENT_CAPSTONE.md) asks for a new, evidence-based report with a manual rubric. Complete it with the worked plan closed and have a knowledgeable person review the reasoning. There is no claim that an actual learner has passed it.

## Verdict

The course supports a path from beginner vocabulary to a capable practitioner of its included labs and advanced reasoning exercises. Calling that universal production mastery would overstate the evidence. The final transfer challenge and supervised practice make the remaining step explicit.

See [validation evidence](VALIDATION.md) for what actually executed.
