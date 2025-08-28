### ✅ Day 19 – Cloud Monitoring & Logging

**📖 Learning Goals**
- Understand **Cloud Monitoring** concepts (metrics, dashboards, SLOs).
- Learn how to configure **alerting policies** for uptime, latency, and errors.
- Explore **Cloud Logging** and create **log-based metrics**.
- Build operational visibility using **Golden Signals** (Latency, Traffic, Errors, Saturation).
- Learn about **Error Budgets** and why they matter for reliability.

---

**📝 Tasks**
- [ ] Read about **Uptime checks, SLOs, and alerting policies** in Cloud Monitoring.  
  👉 [Docs: Uptime checks](https://cloud.google.com/monitoring/uptime-checks)  
  👉 [Docs: SLO Monitoring](https://cloud.google.com/stackdriver/docs/solutions/slo-monitoring)  

- [ ] Explore **Cloud Logging basics**:  
  👉 [Docs: Log Explorer](https://cloud.google.com/logging/docs/view/overview)  
  👉 [Docs: Log-based Metrics](https://cloud.google.com/logging/docs/logs-based-metrics)  

- [ ] Create **custom dashboards** to monitor:  
  - Latency (p95 or p99 response times)  
  - Error Rate (HTTP 5xx or app errors)  
  - Saturation (CPU / memory usage)  

- [ ] Configure **alerting policies**:  
  - Uptime check for a Cloud Run / GKE app endpoint  
  - Alert for high error rates (>5%)  
  - Alert for high CPU (>80%)  

- [ ] Create a **log-based metric** for failed login attempts or HTTP 500 errors.

---

**🧪 Lab – Dashboards + Alerts**
1. Deploy a simple app (Cloud Run or GKE).
2. Set up an **Uptime check** for the app’s endpoint.
3. Create a dashboard with Golden Signals (latency, errors, CPU).
4. Add an **alerting policy** (send email/Slack when thresholds are breached).
5. Define a **log-based metric** and chart it in the dashboard.

---

**💻 CLI Practice**
- Create uptime check via gcloud:
  ```bash
  gcloud monitoring uptime-checks create http my-uptime-check \
    --host=my-app-url.run.app \
    --path=/healthz \
    --period=60s
  ```

---

**🎥 Recommended Udemy Course**

Google Cloud Operations Suite (Stackdriver) for Beginners

Covers Cloud Monitoring, Logging, Dashboards, Alerts, and Best Practices.

---

**🎯 Milestone Check**

- Can you explain Golden Signals and why they matter?
- Can you create an Uptime Check and link it to an alerting policy?
- Did you build at least one custom log-based metric?
- Do you have a dashboard with alerts running for your app?
- Can you trigger an alert (simulate CPU spike or error) and verify notifications?

---

**📊 Outcome**

By the end of Day 19, you will be able to:

- Monitor app uptime, latency, and error rates.
- Define and enforce SLOs with alerting policies.
- Create custom log-based metrics for deeper insights.
- Build dashboards that follow the Golden Signals framework.
- Get proactive alerts via email/Slack before users notice issues.