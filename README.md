# NestJS Board API

**NestJS 기반 게시판 API 프로젝트**  
NestJS의 기본 구조와 개념(Module, Controller, Service, DI 등)을 학습하고,  
CRUD 게시판 API를 구현하며 실무에서 자주 사용하는 기능들을 적용한 토이 프로젝트입니다.  

---

## 주요 기능
- 게시글 CRUD (생성, 조회, 수정, 삭제)
- DTO를 통한 데이터 유효성 검증 (Validation)
- Custom Decorator 활용
- 예외 처리 (Exception Filters)
- 로깅 처리 (Logger Module)
- 환경 변수 관리 (Config Module)
- Swagger를 이용한 API 문서화

---

## 기술 스택
- **Framework**: NestJS (Node.js 기반)  
- **Language**: TypeScript  
- **Database**: (예시) PostgreSQL / MySQL / MongoDB 중 선택  
- **ORM**: TypeORM (or Prisma)  
- **Docs**: Swagger  

---

## 프로젝트 구조 (예시)

```bash
nestjs-board/
├── src/
│   ├── boards/              # 게시판 모듈
│   │   ├── boards.controller.ts
│   │   ├── boards.service.ts
│   │   ├── boards.module.ts
│   │   ├── dto/             # DTO 정의
│   │   └── entities/        # 엔티티 정의
│   ├── common/              # 공통 모듈 (logger, filters, decorators 등)
│   ├── app.module.ts
│   └── main.ts
├── test/
├── package.json
└── tsconfig.json



# NestJS CLI 설치 (처음 1회)
pnpm add -g @nestjs/cli

# 의존성 설치
pnpm install

# 개발 서버 실행
pnpm start:dev



---

## API 문서 (Swagger)

서버 실행 후 브라우저에서 확인:

[http://localhost:3000/api](http://localhost:3000/api)

---

## 향후 개선 방향
- 사용자 인증/인가 (JWT + Passport) 적용  
- 댓글/대댓글 기능 확장  
- RBAC(Role-Based Access Control) 적용  
- 배포 환경 분리(dev, staging, prod)  

---
