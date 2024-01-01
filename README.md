# React + Vite
# [Hosted link](https://markdown-editor-svv3-pk4xp72n7-srivatsas-projects-524d5a78.vercel.app/)
____
## version conflicts.
Installing dependencies like <br>
1. react-md
2. showdown
   etc gave version conflicts.
<br>
"--legacy-peer-peds" was added at end of each install statement to resolve conflicts for local deployment,
<br>
BUT!!!  for deploying remotely in github, bercel or netlify running builds again use normal install statements, instead of peer deps ones.
<br>
so, we need to add a ".npmrc" file with 'legacy-peer-deps=true' passed as instruction for all install commands run locally or remotely.
<br>
add this into your deployment build and all will be good!!

_______

happy coding!!

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
