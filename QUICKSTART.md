# ⚡ Quickstart Guide

## 5-Minute Setup

### 1. Clone & Install

```bash
git clone https://github.com/GlacierEQ/github-repo-enrichment-engine.git
cd github-repo-enrichment-engine
pip install -r requirements.txt
```

### 2. Configure GitHub Token

```bash
# Create token at: https://github.com/settings/tokens
# Required scopes: repo, workflow

export GITHUB_TOKEN="ghp_your_token_here"
```

### 3. Scan Your Repos

```bash
python enrichment_engine.py --owner YourUsername --scan
```

### 4. Deploy Legal Doc Gundam

```bash
python enrichment_engine.py \
  --owner YourUsername \
  --repos "repo1,repo2,repo3" \
  --package legal-doc-gundam
```

### 5. Check Results

Visit:
- `https://github.com/YourUsername/repo1/tree/feature/legal-doc-gundam-integration`
- `https://github.com/YourUsername/repo2/tree/feature/legal-doc-gundam-integration`
- `https://github.com/YourUsername/repo3/tree/feature/legal-doc-gundam-integration`

---

## What Just Happened?

You just deployed:
- ✅ **Evidence-aware document drafter** - No more hallucinations
- ✅ **Multi-jurisdiction support** - HI, CAND, CA9 ready
- ✅ **Quality test suite** - Automated regression testing
- ✅ **Smart AI routing** - Best model for each task
- ✅ **Court profiles** - Complete compliance specs

All production-ready, all in under 5 minutes.

---

## Next Steps

### Create Pull Requests

```bash
# For each repo
gh pr create \
  --repo YourUsername/repo1 \
  --head feature/legal-doc-gundam-integration \
  --base main \
  --title "Add Legal Doc Gundam Integration" \
  --body "Production-grade legal automation suite"
```

### Merge & Deploy

```bash
gh pr merge --merge  # or --squash or --rebase
```

### Start Using

```python
from core.evidence_aware_drafter import EvidenceRegistry, EvidenceAwareDrafter

registry = EvidenceRegistry()
drafter = EvidenceAwareDrafter(registry)

# Zero-hallucination drafting engaged! 🚀
```

---

## Troubleshooting

**Error: GitHub token not found**
```bash
export GITHUB_TOKEN="your_token"
```

**Error: Permission denied**
- Check token has `repo` and `workflow` scopes

**Error: Branch already exists**
- Delete old feature branch first
- Or use `--force` flag

---

## Get Help

- [Full Documentation](README.md)
- [Architecture Guide](docs/ARCHITECTURE.md)
- [Package Development](docs/PACKAGES.md)
- [GitHub Issues](https://github.com/GlacierEQ/github-repo-enrichment-engine/issues)

---

*You're now armed with automated repo enrichment. Go dominate.* 🚀
