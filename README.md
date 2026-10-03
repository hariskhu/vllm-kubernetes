# Plan For This Project
1. Run vLLM locally with a small model in Docker, hit the endpoint
2. Add Grafana, track latency and performance metrics, add load with k6 on cheap cloud GPU
3. Add API gateway (Go): API key auth, rate limits, request metrics, maybe ttimeouts
4. Run locally on kind with a fake inference server (premade responses, artificial delay)
5. Terraform and EKS at the end to save on cloud costs (get the cluster working with fake inference, then run with GPU and real models)
