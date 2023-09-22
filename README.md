1.npm install husky --save-dev
2.npm pkg set scripts.prepare="husky install"
npm run prepare
3.npm pkg set scripts.pre-commit="npm run format && next lint && git add -A ."
4.npx husky add .husky/pre-commit "npm run pre-commit"

5.วิธีใช้ให้ ทำ git commit -m "ข้อความ" ก่อน commit จะมีการ formatcode และ check eslint  