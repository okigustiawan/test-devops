### 7. Deploy sebuah project yang telah Kami sediakan ke Heroku menggunakan heroku-cli sertakan screenshot dan deskripsikan step by step-nya atau record menjadi video.

git clone -b master https://github.com/sgnd/todo-app.git

cd todo-app (masuk ke dir todo-app)

heroku login

heroku create

hapus yang .git di todo-app

git init (membuat .git baru)

heroku git:remote -a warm-stream-15373

git add .

git commit -m "belajar"

git push heroku master

link https://warm-stream-15373.herokuapp.com/
