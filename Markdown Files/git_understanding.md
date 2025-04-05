
# 🔀 Merge Conflicts & Conflict Resolution Reflection

## 🧨 What Caused the Conflict?

I created a merge conflict by editing the same line of a file in two branches:

1. In the `main` branch, I changed a line in `example.txt` to say:
```text
Version from main branch.
```

2. Then in a new branch `feature-branch`, I changed the **same line** to:
```text
Version from feature branch.
```

When I tried to merge `feature-branch` into `main`, Git couldn't auto-merge because it didn’t know which version to keep.

---

## 🛠️ How I Resolved the Conflict

- Git marked the file with conflict indicators:
```text
<<<<<<< HEAD
Version from main branch.
=======
Version from feature branch.
>>>>>>> feature-branch
```

- I manually edited the file to choose the correct version or combine them.
- Then I:
  - Saved the file
  - Used the Git desktop client to mark the conflict as resolved
  - Committed the merge

---

## 📘 What I Learned

- Merge conflicts happen when Git can’t automatically reconcile changes made to the same part of a file.
- They’re common in collaborative environments or when working on long-lived branches.
- Resolving them involves:
  - Carefully reviewing the conflicting changes
  - Choosing or merging the correct lines
  - Marking the conflict as resolved and committing

### 🔍 Tips:
- Communicate clearly with teammates to avoid overlapping changes.
- Pull and sync often to stay up to date.
- Use tools like VS Code or Git GUI clients to resolve conflicts more easily.

---

## ✅ Final Thoughts

Experiencing and resolving a merge conflict helped me understand Git's version control at a deeper level. It taught me how to carefully review changes, use Git’s conflict markers, and ensure code integrity while collaborating on shared codebases.
