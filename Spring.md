spring Research
==============

# 1. Spring이란
Spring은 웹 쪽에서 많이 쓰이고 있어서 자바를 이용한 웹 프레임워크라고 생각하고 있었다(심지어 학교에서 스프링을 활용하는 수업을 들었는데도 말이다). 하지만 본격적으로 관심을 가지고 알아보니 단순히 웹 만을 위한 프레임워크는 아니였으며, 핵심기능인 IoC와 DI를 쓰기 위한 프레임워크라고 정의할 수도 없을 것 같다. 개인적으로 스프링은 좋은 디자인 패턴들을 쉽게 사용하기 위해 이리저리 묶어놓은 프레임워크라고 생각한다. 이것이 웹 개발하는데 편리하여 웹에서 많이 쓰이는 것 같다.

# 2. Spring을 써보자
Spring을 그래서 한 번 써보기로 하였다. 예전 이클립스에서 STS를 활용하여 개발하였을때 자주 열받았던 기억이 있어서 IntelliJ를 활용하기로 하였다. 헌데 구글에 Spring을 설정하는 법들을 찾아보니 블로그들마다 전부 제각기 다른 방법으로 설정하고 있었다. 버전업이 되면서 바뀌는 부분들이 있는 듯 하였다. 일단 아파치가 필요하다. 아파치 홈페이지에서 원하는 버전을 받아주면 되는데 나는 제일 최신인 9버전을 받았다. 그리고 IntelliJ에서 Maven 카테고리를 선택하여 maven-archetype-webapp을 선택해준다. 
![spring01](HackdayResearch/images/2-spring/spring01.png)

GroupId와 ArtifactId를 설정해준다. 
![spring02](https://github.com/cosmicb0y/images/2-spring/spring02.png)

maven을 세팅하는 창을 나오는데 그냥 기본설정으로 넘어가면 된다. 
![spring03](https://github.com/cosmicb0y/images/2-spring/spring03.png)

project name도 원하는 대로 설정해주면 된다.

프로젝트에 Add Framework Support를 해준다.
![spring04](https://github.com/cosmicb0y/images/2-spring/spring04.png)

Spring MVC를 선택해준다.
![spring05](https://github.com/cosmicb0y/images/2-spring/spring05.png)

서버를 가동시키기 위해 Edit Configuration을 해준다.
![spring06](https://github.com/cosmicb0y/images/2-spring/spring06.png)

톰캣을 골라주고 Deployment에서 웹 서버를 선택해주고 Apply해준다.
![spring07](https://github.com/cosmicb0y/images/2-spring/spring07.png)
![spring08](https://github.com/cosmicb0y/images/2-spring/spring08.png)
![spring09](https://github.com/cosmicb0y/images/2-spring/spring09.png)

그리고 Run을 해주면 톰캣서버 화면이 뜬다.
![spring10](https://github.com/cosmicb0y/images/2-spring/spring10.png)


# 3. 초기설정이 귀찮아
그리고 여기에서 사용하고 싶은 기능이 있다면 pom.xml에 dependency들을 추가시켜주어야한다. 초기설정이 상당히 할게 많아서 귀찮은데 이러한 점을 쉽게 해주는 것이 Springboot이다. springboot로 spring 프로젝트를 만드는 방법은 다음과 같다.

프로젝트에서 Spring Initializr를 선택한다.
![springboot01](https://github.com/cosmicb0y/images/3-springboot/springboot1.png)

Group과 Artifact를 설정해준다. Maven을 할지 Gradle을 할지 정해야하는데 Maven을 선택해주었다. Gradle이 더 빠르다고 하지만 새롭게 문법을 익혀야하므로 일단 xml로 설정이 편하게 가능한 Maven을 쓰기로 했다.
![springboot02](https://github.com/cosmicb0y/images/3-springboot/springboot2.png)

Dependency들을 골라준다. 일단은 필요한게 없으므로 그냥 넘어갔다.
![springboot03](https://github.com/cosmicb0y/images/3-springboot/springboot3.png)

프로젝트 이름을 설정해준다.
![springboot04](https://github.com/cosmicb0y/images/3-springboot/springboot4.png)

그럼 짠 끝이다.

완전 편하므로 springboot를 쓰기로 했다.