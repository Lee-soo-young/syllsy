Untitled
================

# R을 이용한 웹페이지

## 작성자 소개

### 이수영

내 이름은 “뛰어난 재주를 받아 꽃과같은 사람이 되어라” 라는 뜻이다. \#\#\# 사회학과 사회학과는 “사회와 인간의 관계”를
배우는 학과이다. \#\#\# 좋아하는 것들 + 친구 - 유시연 중2때 같은 반 친구 - 안유진 안뉴라는 별명을 가진 이친구는
이름보다 별명을 더 많이 부른다. + 애착 물건 - 스마트폰 요즘은 스마트폰 없이는 살기 힘든것 같다. - + 음식 - 계란
계란으로 만든 요리는 정말 맛있다. - 커피 얼어죽어도 아이스 아메리카노를 먹어야겠다.

![성규](img/캡처.png)

\#자료 분석

\#\#ggplot2 의 mpg 데이터

패키지 불러옵니다.

``` r
library(ggplot2)
```

우리는 자동차 경비 데이터인 mpg 데이터를 이용하여 배기량과 도시연비의 관계를 그래프로 살펴보았다.

먼저 mpg패키지를 살펴보겠습니다.

``` r
head(mpg,10)
```

    ## # A tibble: 10 x 11
    ##    manufacturer model displ  year   cyl trans drv     cty   hwy fl    class
    ##    <chr>        <chr> <dbl> <int> <int> <chr> <chr> <int> <int> <chr> <chr>
    ##  1 audi         a4      1.8  1999     4 auto~ f        18    29 p     comp~
    ##  2 audi         a4      1.8  1999     4 manu~ f        21    29 p     comp~
    ##  3 audi         a4      2    2008     4 manu~ f        20    31 p     comp~
    ##  4 audi         a4      2    2008     4 auto~ f        21    30 p     comp~
    ##  5 audi         a4      2.8  1999     6 auto~ f        16    26 p     comp~
    ##  6 audi         a4      2.8  1999     6 manu~ f        18    26 p     comp~
    ##  7 audi         a4      3.1  2008     6 auto~ f        18    27 p     comp~
    ##  8 audi         a4 q~   1.8  1999     4 manu~ 4        18    26 p     comp~
    ##  9 audi         a4 q~   1.8  1999     4 auto~ 4        16    25 p     comp~
    ## 10 audi         a4 q~   2    2008     4 manu~ 4        20    28 p     comp~
