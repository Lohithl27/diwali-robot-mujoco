# Push to GitHub (from your MacBook Terminal)

1. On github.com click New repository. Name: `diwali-robot-mujoco`. Public. Do NOT add a README, .gitignore or license (they already exist here). Click Create.
2. In Terminal:

```bash
cd ~/Downloads/diwali-robot-mujoco
git init -b main
git add .
git commit -m "Diwali robot: UR5e writes Kannada wishes and launches a rocket in MuJoCo"
git remote add origin https://github.com/<YOUR_USERNAME>/diwali-robot-mujoco.git
git push -u origin main
```
If asked for a password, use a Personal Access Token (GitHub > Settings > Developer settings > Tokens) or run `gh auth login` first.
3. Add repo topics: robotics, mujoco, ur5e, simulation, python, diwali, kannada.
