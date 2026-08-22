# Arquitetura do backend

> Comando Tree na raiz do projeto

```text
src/
├── config
│   ├── MongoConfig.java
│   └── SecurityConfig.java
├── exception
│   ├── ApiException.java
│   ├── ConflictException.java
│   ├── ErrorMessages.java
│   ├── ErrorResponse.java
│   ├── ForbiddenException.java
│   └── GlobalExceptionHandler.java
├── FitsyncApiApplication.java
├── modules
│   ├── auth
│   │   ├── controller
│   │   │   └── AuthController.java
│   │   ├── dto
│   │   │   ├── AuthResponseDTO.java
│   │   │   ├── AuthResponseMeDTO.java
│   │   │   ├── LoginDTO.java
│   │   │   ├── LogoutRequestDTO.java
│   │   │   ├── RefreshRequestDTO.java
│   │   │   └── RegisterDTO.java
│   │   ├── entity
│   │   │   ├── EmailVerificationToken.java
│   │   │   └── RefreshToken.java
│   │   ├── exception
│   │   │   ├── EmailNotVerifiedException.java
│   │   │   ├── InvalidCredentialsException.java
│   │   │   ├── InvalidRefreshTokenException.java
│   │   │   └── UserAlreadyExistsException.java
│   │   ├── repository
│   │   │   ├── EmailVerificationTokenRepository.java
│   │   │   └── RefreshTokenRepository.java
│   │   ├── security
│   │   │   ├── AuthEntryPoint.java
│   │   │   ├── AuthorizationService.java
│   │   │   ├── JwtAuthenticationFilter.java
│   │   │   └── TokenService.java
│   │   └── service
│   │       ├── AuthService.java
│   │       ├── EmailService.java
│   │       └── RefreshTokenService.java
│   ├── user
│   │   ├── linkRequest
│   │   │   ├── controller
│   │   │   │   └── LinkRequestController.java
│   │   │   ├── dto
│   │   │   │   └── LinkProfessionalDTO.java
│   │   │   ├── entity
│   │   │   │   └── LinkRequest.java
│   │   │   ├── enums
│   │   │   │   └── LinkStatus.java
│   │   │   ├── exception
│   │   │   │   └── LinkRequestNotFoundException.java
│   │   │   ├── repository
│   │   │   │   └── LinkRequestRepository.java
│   │   │   └── service
│   │   │       └── LinkRequestService.java
│   │   └── user
│   │       ├── controller
│   │       │   └── UserController.java
│   │       ├── dto
│   │       │   ├── ClientProfileResponseDTO.java
│   │       │   ├── ProfessionalProfileResponseDTO.java
│   │       │   ├── UpdateClientProfileDTO.java
│   │       │   ├── UpdateProfessionalProfileDTO.java
│   │       │   └── UpdateProfileDTO.java
│   │       ├── entity
│   │       │   ├── ClientProfile.java
│   │       │   ├── ProfessionalProfile.java
│   │       │   └── User.java
│   │       ├── enums
│   │       │   ├── BiologicalSex.java
│   │       │   └── Role.java
│   │       ├── exception
│   │       │   └── ProfileNotFoundException.java
│   │       ├── repository
│   │       │   ├── ClientProfileRepository.java
│   │       │   ├── ProfessionalProfileRepository.java
│   │       │   └── UserRepository.java
│   │       └── service
│   │           └── UserService.java
│   └── workout
│       ├── exercise
│       │   ├── controller
│       │   │   └── ExerciseController.java
│       │   ├── dto
│       │   │   ├── ExerciseRequestDTO.java
│       │   │   └── UpdateExerciseDTO.java
│       │   ├── entity
│       │   │   └── Exercise.java
│       │   ├── enums
│       │   │   └── MuscleGroup.java
│       │   ├── exception
│       │   │   └── ExerciseNotFoundException.java
│       │   ├── repository
│       │   │   └── ExerciseRepository.java
│       │   └── service
│       │       └── ExerciseService.java
│       ├── trainingPlan
│       │   ├── controller
│       │   │   └── TrainingPlanController.java
│       │   ├── dto
│       │   │   ├── TrainingPlanRequestDTO.java
│       │   │   └── UpdateTrainingPlanDTO.java
│       │   ├── entity
│       │   │   └── TrainingPlan.java
│       │   ├── exception
│       │   │   └── TrainingPlanNotFoundException.java
│       │   ├── repository
│       │   │   └── TrainingPlanRepository.java
│       │   └── service
│       │       └── TrainingPlanService.java
│       └── workout
│           ├── controller
│           │   └── WorkoutController.java
│           ├── dto
│           │   ├── UpdateWorkoutDTO.java
│           │   └── WorkoutRequestDTO.java
│           ├── entity
│           │   └── Workout.java
│           ├── exception
│           │   └── WorkoutNotFoundException.java
│           ├── repository
│           │   └── WorkoutRepository.java
│           └── service
│               └── WorkoutService.java
└── util
    └── UpdateUtils.java
```