# xAI Grok vs GLM-4 Coding Comparison 📊

## Benchmarks (Latest Available)
| Benchmark     | xAI Grok-4.1/4.20 | GLM-4 / GLM-4.7 | Notes |
|---------------|-------------------|-----------------|-------|
| **HumanEval** | ~90-95% (saturates) | 94.2%          | Code gen pass@1 |
| **LiveCodeBench** | High (multi-agent) | 84.9%        | Real-world code exec/repair |
| **MBPP**      | Leaderboard top  | Competitive    | Python problems |
| **SWE-Bench** | N/A               | Strong agent   | Software eng tasks |
| **Context**   | 128K+ tokens     | 128K tokens    | - |

**Sources:** LMSYS, ArtificialAnalysis, Z.ai blog, x.ai.

## Pricing Formula (per 1M Tokens)
```
xAI Grok-4.1 Fast: Input $0.20 + Output $0.50
GLM-4 API: ~$0.10 input + $0.30 output (Zhipu; free local open-source)
Cost Ratio = GLM / xAI ≈ 0.5x (cheaper for volume)
```

## Pros/Cons Formula
**xAI Grok:** Multi-agent reasoning 🚀 + Fast inference + xAI ecosystem  
**GLM-4:** Open-source free local ⚡ + Strong Chinese/eng bi-lingual + Agentic  

**Choose GLM if:** Open/local, cost-sensitive.  
**Choose xAI if:** Cutting-edge benchmarks, integrated tools.

**Est. coding task:** xAI ~$0.01 (10K tok), GLM ~$0.005