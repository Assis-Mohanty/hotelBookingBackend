"# hotelBookingBackend" 

FileTree:

```
├── AuthService
│   ├── app
│   │   └── app.go
│   ├── config
│   │   ├── db
│   │   │   └── db.go
│   │   ├── db.go
│   │   └── env.go
│   ├── controllers
│   │   ├── ping.controller.go
│   │   └── user.controller.go
│   ├── db
│   │   ├── migrations
│   │   │   └── 20251231213830_add_user_table.sql
│   │   └── repository
│   │       ├── storage.go
│   │       └── user.repository.go
│   ├── middlewares
│   │   ├── jwtVerify.middleware.go
│   │   ├── middleware.go
│   │   └── rateLimiter.go
│   ├── models
│   │   └── user.model.go
│   ├── routes
│   │   ├── routes.go
│   │   └── user.router.go
│   ├── services
│   │   └── user.service.go
│   ├── utils
│   │   ├── hash.go
│   │   ├── jsonEncoder.go
│   │   └── reverseProxy.go
│   ├── Makefile
│   ├── README.md
│   ├── e.exe
│   ├── go.mod
│   ├── go.sum
│   └── main.go
├── BookingService
│   ├── logs
│   │   └── .f63e9e54b8cfddbdfb306dd93044e79161bf7288-audit.json
│   ├── src
│   │   ├── config
│   │   │   ├── index.ts
│   │   │   ├── logger.config.ts
│   │   │   └── redisConfig.ts
│   │   ├── controllers
│   │   │   ├── booking.controller.ts
│   │   │   └── ping.controller.ts
│   │   ├── dto
│   │   │   ├── booking.dto.ts
│   │   │   └── notification.dto.ts
│   │   ├── middlewares
│   │   │   ├── correlation.middleware.ts
│   │   │   └── error.middleware.ts
│   │   ├── prisma
│   │   │   ├── migrations
│   │   │   │   ├── 20251015125458_init
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251015125905_added_total_guest_in_booking
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251015141216_added_total_guest_in_bookingq
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251015141232_added_total_guest_in_bookingqq
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251015154854_added_idempotency_key_model
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251015195639_added_total_guest_in_bookingqqqqq
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251018073525_updated_prisma_model
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251021090952_updatedqq
│   │   │   │   │   └── migration.sql
│   │   │   │   ├── 20251106135640_update_booking_model
│   │   │   │   │   └── migration.sql
│   │   │   │   └── migration_lock.toml
│   │   │   ├── client.ts
│   │   │   └── schema.prisma
│   │   ├── producer
│   │   │   └── email.producer.ts
│   │   ├── queue
│   │   │   └── queue.ts
│   │   ├── repository
│   │   │   └── booking.repository.ts
│   │   ├── routers
│   │   │   ├── v1
│   │   │   │   ├── booking.router.ts
│   │   │   │   ├── index.router.ts
│   │   │   │   └── ping.router.ts
│   │   │   └── v2
│   │   │       └── index.router.ts
│   │   ├── services
│   │   │   └── booking.service.ts
│   │   ├── utils
│   │   │   ├── errors
│   │   │   │   └── app.error.ts
│   │   │   └── helpers
│   │   │       ├── generateIdempotencyKey.ts
│   │   │       └── request.helpers.ts
│   │   ├── validators
│   │   │   ├── booking.validator.ts
│   │   │   ├── index.ts
│   │   │   └── ping.validator.ts
│   │   ├── .gitignore
│   │   └── server.ts
│   ├── .gitignore
│   ├── README.md
│   ├── package-lock.json
│   ├── package.json
│   ├── test.csv
│   └── tsconfig.json
├── HotelService
│   ├── logs
│   │   └── .f63e9e54b8cfddbdfb306dd93044e79161bf7288-audit.json
│   ├── src
│   │   ├── config
│   │   │   ├── config.js
│   │   │   ├── config.json
│   │   │   ├── index.ts
│   │   │   ├── logger.config.ts
│   │   │   ├── q.js
│   │   │   └── sequelize.config.js
│   │   ├── controllers
│   │   │   ├── hotel.controler.ts
│   │   │   ├── ping.controller.ts
│   │   │   └── roomCategory.controller.ts
│   │   ├── dto
│   │   │   ├── hotel.dto.ts
│   │   │   └── roomCategory.dto.ts
│   │   ├── middlewares
│   │   │   ├── correlation.middleware.ts
│   │   │   └── error.middleware.ts
│   │   ├── migrations
│   │   │   ├── 20250902184312-create-hotel-table.js
│   │   │   ├── 20250903171806-add-ratings-hotel-table.js
│   │   │   ├── 20250906045308-add-deleted_at-column-to-hotels-table.js
│   │   │   ├── 20251104172847-updating_hotelModel.js
│   │   │   ├── 20251104190909-create-room.js
│   │   │   ├── 20251105153101-update_room_number.js
│   │   │   ├── 20251105231020-update.js
│   │   │   └── 20251107160801-create-room.js
│   │   ├── models
│   │   │   ├── association.model.ts
│   │   │   ├── hotel.ts
│   │   │   ├── index.js
│   │   │   ├── room.ts
│   │   │   ├── roomCategory.ts
│   │   │   └── sequelize.ts
│   │   ├── repository
│   │   │   ├── baseRepository.ts
│   │   │   ├── hotel.respository.ts
│   │   │   ├── room.repository.ts
│   │   │   └── roomCategory.repository.ts
│   │   ├── routers
│   │   │   ├── v1
│   │   │   │   ├── hotel.router.ts
│   │   │   │   ├── index.router.ts
│   │   │   │   ├── ping.router.ts
│   │   │   │   └── room.router.ts
│   │   │   └── v2
│   │   │       └── index.router.ts
│   │   ├── seeders
│   │   ├── services
│   │   │   ├── hotel.service.ts
│   │   │   └── roomCategory.service.ts
│   │   ├── utils
│   │   │   ├── errors
│   │   │   │   └── app.error.ts
│   │   │   └── helpers
│   │   │       └── request.helpers.ts
│   │   ├── validators
│   │   │   ├── hotel.validator.ts
│   │   │   ├── index.ts
│   │   │   ├── ping.validator.ts
│   │   │   └── room.validator.ts
│   │   └── server.ts
│   ├── .gitignore
│   ├── .sequelizerc
│   ├── README.md
│   ├── package-lock.json
│   ├── package.json
│   └── tsconfig.json
├── NotificationService
│   ├── logs
│   │   └── .f63e9e54b8cfddbdfb306dd93044e79161bf7288-audit.json
│   ├── src
│   │   ├── config
│   │   │   ├── email.config.ts
│   │   │   ├── index.ts
│   │   │   ├── logger.config.ts
│   │   │   └── redis.config.ts
│   │   ├── controllers
│   │   │   └── ping.controller.ts
│   │   ├── dto
│   │   │   └── notification.dto.ts
│   │   ├── middlewares
│   │   │   ├── correlation.middleware.ts
│   │   │   └── error.middleware.ts
│   │   ├── prisma
│   │   │   └── schema.prisma
│   │   ├── producer
│   │   │   └── email.producer.ts
│   │   ├── publisher
│   │   │   └── email.publisher.ts
│   │   ├── queue
│   │   │   └── queue.ts
│   │   ├── routers
│   │   │   ├── v1
│   │   │   │   ├── index.router.ts
│   │   │   │   └── ping.router.ts
│   │   │   └── v2
│   │   │       └── index.router.ts
│   │   ├── service
│   │   │   └── mailer.service.ts
│   │   ├── template
│   │   │   ├── mailer
│   │   │   │   └── email.mailer.hbs
│   │   │   └── template.ts
│   │   ├── utils
│   │   │   ├── errors
│   │   │   │   └── app.error.ts
│   │   │   └── helpers
│   │   │       └── request.helpers.ts
│   │   ├── validators
│   │   │   ├── index.ts
│   │   │   └── ping.validator.ts
│   │   ├── .gitignore
│   │   ├── prisma.config.ts
│   │   └── server.ts
│   ├── .gitignore
│   ├── README.md
│   ├── package-lock.json
│   ├── package.json
│   └── tsconfig.json
└── README.md
```

---
