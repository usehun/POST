# POST
 nomard Youtube Code Challenge 6

```
(1) movieRouter.js에 작성한 movieRouter.route("/add").get(add).post(add)
  하나의 라우트에 GET과 POST를 요청을 함께 사용하려면 router.route() 메서드를 사용하면 됩니다.
  (주의) GET과 POST 요청을 처리하는/add URL에 대한 라우트는 반드시 /:id 라우트 보다 위에 작성해야 합니다.

(2) movieController.js에 작성한 add 컨트롤러는 req.method가 GET인 경우 add 페이지를 렌더 하고,
  req.method가 POST인 경우 사용자가 작성한 새로운 영화를 DB에 추가하는 함수입니다.
  if else 구문을 사용하여 req.method가 GET인 경우 add.pug를 렌더 합니다.
  POST인 경우 사용자가 입력한 form의 값을 req.body로 가져올 수 있습니다.
  const { body: { title, genres, synopsis } } = req
  addMovie({ title, synopsis, genres: genres.split(",") });
  req.body 값을 객체로 가져와 addMovie()함수의 인자로 보내면 사용자가 입력한 값의 영화가 DB에 추가됩니다.
  genres.split(",")
  String.split() 메서드를 사용하면 장르 입력 시 ,로 단어를 구분하여 genres 배열에 각 단어가 각 요소 분할되어 들어갑니다.
```
