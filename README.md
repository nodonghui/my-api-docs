# API Documentation

## Overview
This is the documentation for the API of [Project Name].

## Endpoints

### GET /users
Fetch all users.

**Request Example:**
```bash
curl -X GET https://api.example.com/users

Response Example:
{
  "users": [
    {
      "id": 1,
      "name": "John Doe"
    }
  ]
}
```
POST /users
Create a new user.

Request Example:

curl -X POST https://api.example.com/users -d '{"name": "Jane Doe"}'

{
  "id": 2,
  "name": "Jane Doe"
}
### 3. GitHub Pages 설정

1. 리포지토리의 **Settings** 탭으로 이동합니다.
2. 왼쪽 메뉴에서 **Pages**를 클릭합니다.
3. **Source** 섹션에서 **Branch**를 `main` 또는 `master`로 선택하고, 폴더는 `root`로 설정합니다.
4. **Save**를 클릭합니다.

GitHub Pages는 이제 `main` 브랜치의 루트 디렉토리에 있는 Markdown 파일을 자동으로 웹 페이지로 변환하여 제공합니다.

### 4. 문서 HTML로 변환

Markdown 파일을 HTML 형식으로 변환하려면 GitHub Pages에서 기본적으로 제공하는 **Jekyll**이라는 정적 사이트 생성기를 사용할 수 있습니다.

1. 리포지토리의 루트에 `_config.yml` 파일을 생성하고, 아래와 같은 내용을 추가합니다.

```yaml
title: My API Documentation
theme: jekyll-theme-cayman
