---
title: "Hugo로 기술 블로그 만들기"
date: 2026-05-03
description: "카테고리, 태그, 번역 연결, KaTeX 렌더링을 확인하는 첫 한국어 글입니다."
contentLang: "ko"
categories: ["블로그"]
tags: ["hugo", "수학", "검색"]
draft: false
math: true
translationKey: "hello-hugo"
---

이 글은 블로그의 핵심 작성 기능을 확인합니다. Markdown 본문, 분류, 번역 연결, 검색 인덱싱, 수식 렌더링을 함께 점검합니다.

## 수식 렌더링

문장 안의 인라인 수식은 $E = mc^2$처럼 표시되어야 합니다.

블록 수식은 가운데 정렬된 식으로 표시되어야 합니다.

$$
\int_0^1 x^2\,dx = \frac{1}{3}
$$

## 검색 메타데이터

Pagefind는 이 페이지의 제목, 설명, 태그, 카테고리, 본문을 인덱싱해야 합니다. 서버 없이도 정적 사이트에서 전체 텍스트 검색을 사용할 수 있습니다.
