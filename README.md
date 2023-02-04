# movieapp

### List 구현 화면

리스트 구현 화면은 Public 으로 제공되고 있는 API 중, 다음으로 제공하는 3개의 API중 하나를 선택하여 리스트 형식으로 보여주시면 됩니다.

- Github Users - [https://api.github.com/users](https://api.github.com/users)
    
    ```jsx
    {
        "login": "mojombo",
        "id": 1,
        "node_id": "MDQ6VXNlcjE=",
        "avatar_url": "https://avatars.githubusercontent.com/u/1?v=4",
        "gravatar_id": "",
        "url": "https://api.github.com/users/mojombo",
        "html_url": "https://github.com/mojombo",
        "followers_url": "https://api.github.com/users/mojombo/followers",
        "following_url": "https://api.github.com/users/mojombo/following{/other_user}",
        "gists_url": "https://api.github.com/users/mojombo/gists{/gist_id}",
        "starred_url": "https://api.github.com/users/mojombo/starred{/owner}{/repo}",
        "subscriptions_url": "https://api.github.com/users/mojombo/subscriptions",
        "organizations_url": "https://api.github.com/users/mojombo/orgs",
        "repos_url": "https://api.github.com/users/mojombo/repos",
        "events_url": "https://api.github.com/users/mojombo/events{/privacy}",
        "received_events_url": "https://api.github.com/users/mojombo/received_events",
        "type": "User",
        "site_admin": false
      }
    ```
    
- TMDB API - [https://developers.themoviedb.org/3/getting-started/introduction](https://developers.themoviedb.org/3/getting-started/introduction)
    
    ```jsx
    {
    	"adult":false,
    	"backdrop_path":"/s16H6tpK2utvwDtzZ8Qy4qm5Emw.jpg",
    	"genre_ids":[
    		878,
    		12,
    		28
    	],
    	"id":76600,
    	"original_language":"en",
    	"original_title":"Avatar: The Way of Water",
    	"overview":"Set more than a decade after the events of the first film, learn the story of the Sully family (Jake, Neytiri, and their kids), the trouble that follows them, the lengths they go to keep each other safe, the battles they fight to stay alive, and the tragedies they endure.",
    	"popularity":4718.023,
    	"poster_path":"/t6HIqrRAclMCA60NsSmeqe9RmNV.jpg",
    	"release_date":"2022-12-14",
    	"title":"Avatar: The Way of Water",
    	"video":false,
    	"vote_average":7.7,
    	"vote_count":3562
    },
    ```
    
- DummyJson API - [https://dummyjson.com/docs/products](https://dummyjson.com/docs/products)
    
    ```jsx
    {
          "id": 1,
          "title": "iPhone 9",
          "description": "An apple mobile which is nothing like apple",
          "price": 549,
          "discountPercentage": 12.96,
          "rating": 4.69,
          "stock": 94,
          "brand": "Apple",
          "category": "smartphones",
          "thumbnail": "...",
          "images": ["...", "...", "..."]
    },
    ```
    

이 3개의 API 중 **단 1개의 API** 만을 선택하여 화면을 구성합니다.

> **리스트의 아이템은 무조건 하나의 이미지를 포함하여야 합니다.**
> 

### Detail 구현 화면

정하신 하나의 API에서 하나의 요소를 클릭했을 때, 디테일 페이지로 이동하도록 합니다. 

디테일 페이지에서는 받아온 모델 요소중 중요하다고 생각되는 5개의 요소를 골라 보여주도록 합니다.


## 기술

- Network 사용 기술
    - Retrofit
- List 화면 UI
    - Vertical Linear
