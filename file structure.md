prompt-heist/
│
├── README.md                                      (Shreya)
├── STORIES.md                                     (Shreya)
├── .gitignore                                     (Shreya)
│
├── team/
│   ├── Shreya.md                                  (Shreya)
│   ├── Shravani.md                                (Shravani)
│   ├── Asmita.md                                  (Asmita)
│   ├── Mrudula.md                                 (Mrudula)
│   └── Harsimar.md                                (Harsimar)
│
├── docs/
│   ├── architecture.md                            (Shreya)
│   ├── api-contract.md                            (Shravani, Asmita, Shreya)
│   ├── socket-contract.md                          (Shravani, Asmita)
│   ├── firestore-schema.md                         (Shravani, Asmita)
│   ├── agent-contracts.md                          (Shreya, Shravani, Asmita)
│   ├── local-development.md                        (Shreya)
│   ├── gcp-console-setup.md                        (Shreya)
│   ├── deployment.md                               (Shreya)
│   ├── testing-and-qe.md                           (Suraj)
│   └── reference/
│       ├── game.txt                                (Shreya)
│       ├── PRD.md                                  (Shreya)
│       └── Backend_overview.md                     (Shravani)
│
├── backend/
│   ├── package.json                                (Shreya)
│   ├── package-lock.json                            (Shreya)
│   ├── tsconfig.json                               (Shreya)
│   ├── eslint.config.js                            (Shreya)
│   ├── vitest.config.ts                            (Shreya)
│   ├── Dockerfile                                  (Shreya)
│   ├── .env.example                                (Shreya)
│   │
│   ├── src/
│   │   ├── server.ts                               (Shreya)
│   │   ├── app.ts                                  (Shreya)
│   │   ├── clock.ts                                (Shreya)
│   │   │
│   │   ├── config/
│   │   │   ├── env.ts                              (Shreya)
│   │   │   ├── constants.ts                        (Shreya)
│   │   │   └── model-config.ts                     (Shreya)
│   │   │
│   │   ├── routes/
│   │   │   ├── index.ts                            (Shreya)
│   │   │   ├── controller.routes.ts                (Asmita, Shravani)
│   │   │   ├── player.routes.ts                    (Asmita)
│   │   │   ├── display.routes.ts                   (Shravani)
│   │   │   ├── treasure.routes.ts                  (Shreya)
│   │   │   ├── monitor.routes.ts                   (Shreya, Shravani)
│   │   │   └── event.routes.ts                     (Shreya)
│   │   │
│   │   ├── controllers/
│   │   │   ├── auth.controller.ts                  (Asmita)
│   │   │   ├── session.controller.ts               (Asmita)
│   │   │   ├── player.controller.ts                (Asmita)
│   │   │   ├── prompt.controller.ts                (Shravani)
│   │   │   ├── treasure.controller.ts              (Shreya)
│   │   │   ├── result.controller.ts                (Shravani, Asmita)
│   │   │   ├── event.controller.ts                 (Shreya)
│   │   │   └── monitor.controller.ts               (Shreya)
│   │   │
│   │   ├── services/
│   │   │   ├── auth.service.ts                     (Asmita)
│   │   │   ├── session.service.ts                  (Asmita)
│   │   │   ├── player.service.ts                   (Asmita)
│   │   │   ├── prompt.service.ts                   (Shravani)
│   │   │   ├── scoring.service.ts                  (Shravani)
│   │   │   ├── timer.service.ts                    (Shravani)
│   │   │   ├── result-calculator.service.ts        (Shravani)
│   │   │   ├── treasure.service.ts                (Shreya)
│   │   │   ├── name-review.service.ts              (Shreya)
│   │   │   ├── csv-export.service.ts               (Shreya)
│   │   │   ├── event-cleanup.service.ts             (Shreya)
│   │   │   └── audit.service.ts                    (Shreya, Shravani)
│   │   │
│   │   ├── repositories/
│   │   │   ├── session.repository.ts               (Shravani)
│   │   │   ├── player.repository.ts                (Shravani)
│   │   │   ├── prompt.repository.ts                (Shravani)
│   │   │   ├── treasure.repository.ts              (Shravani, Shreya)
│   │   │   ├── event.repository.ts                 (Shravani)
│   │   │   ├── audit.repository.ts                 (Shravani)
│   │   │   └── controller.repository.ts            (Shravani)
│   │   │
│   │   ├── models/
│   │   │   ├── session.model.ts                    (Asmita)
│   │   │   ├── player.model.ts                     (Asmita)
│   │   │   ├── prompt.model.ts                     (Asmita, Shravani)
│   │   │   ├── treasure.model.ts                   (shra)
│   │   │   ├── event.model.ts                      (Shravani)
│   │   │   └── audit.model.ts                      (Shravani)
│   │   │
│   │   ├── state-machines/
│   │   │   ├── session-state.machine.ts             (Asmita)
│   │   │   ├── player-state.machine.ts              (Asmita)
│   │   │   ├── prompt-state.machine.ts              (Asmita, Shravani)
│   │   │   └── event-state.machine.ts               (Shravani)
│   │   │
│   │   ├── sockets/
│   │   │   ├── socket-server.ts                    (Shravani)
│   │   │   ├── controller.namespace.ts             (Shravani)
│   │   │   ├── player.namespace.ts                 (Shravani)
│   │   │   ├── display.namespace.ts                (Shravani)
│   │   │   ├── socket-auth.ts                      (Asmita)
│   │   │   └── socket-events.ts                    (Shravani, Asmita)
│   │   │
│   │   ├── integrations/
│   │   │   ├── ai-service.client.ts                (Shreya)
│   │   │   ├── firestore.client.ts                 (Shravani)
│   │   │   ├── storage.client.ts                   (Shreya)
│   │   │   └── secret-manager.client.ts            (Shreya)
│   │   │
│   │   ├── middleware/
│   │   │   ├── auth.middleware.ts                  (Asmita)
│   │   │   ├── correlation-id.middleware.ts        (Shreya)
│   │   │   ├── error.middleware.ts                 (Shreya)
│   │   │   ├── rate-limit.middleware.ts            (Shreya)
│   │   │   └── request-validation.middleware.ts    (Asmita)
│   │   │
│   │   ├── interfaces/
│   │   │   ├── clock.interface.ts                  (Shreya)
│   │   │   ├── ai-service.interface.ts             (Shreya)
│   │   │   └── repository.interface.ts             (Shravani)
│   │   │
│   │   └── utils/
│   │       ├── logger.ts                           (Shreya)
│   │       ├── log-redaction.ts                    (Shreya)
│   │       ├── correlation-id.ts                   (Shreya)
│   │       ├── error-codes.ts                      (Shreya, Shravani)
│   │       └── csv-sanitizer.ts                    (Shreya)
│   │
│   └── tests/
│       ├── unit/
│       │   ├── session.service.test.ts              (Asmita)
│       │   ├── player.service.test.ts               (Asmita)
│       │   ├── prompt.service.test.ts               (Shravani)
│       │   ├── scoring.service.test.ts              (Shravani)
│       │   ├── timer.service.test.ts                (Shravani)
│       │   ├── result-calculator.test.ts            (Shravani)
│       │   ├── treasure.service.test.ts             (Shreya)
│       │   ├── event-cleanup.test.ts                (Shreya)
│       │   ├── csv-export.test.ts                   (Shreya)
│       │   └── log-redaction.test.ts                (Shreya)
│       │
│       └── integration/
│           ├── auth.integration.test.ts             (Asmita)
│           ├── session.integration.test.ts          (Asmita)
│           ├── player-join.integration.test.ts      (Asmita)
│           ├── prompt-flow.integration.test.ts      (Shravani)
│           ├── treasure-flow.integration.test.ts    (Shreya)
│           └── event-close.integration.test.ts      (Shreya)
│
├── ai-service/
│   ├── requirements.txt                            (Shreya)
│   ├── Dockerfile                                  (Shreya)
│   ├── .env.example                                (Shreya)
│   │
│   ├── app/
│   │   ├── __init__.py                             (Shreya)
│   │   ├── main.py                                 (Shreya)
│   │   ├── config.py                               (Shreya)
│   │   ├── dependencies.py                         (Shreya)
│   │   │
│   │   ├── api/
│   │   │   ├── __init__.py                         (Shreya)
│   │   │   ├── router.py                           (Shreya)
│   │   │   ├── health.py                           (Shreya)
│   │   │   ├── filter_routes.py                    (Shreya)
│   │   │   ├── guard_routes.py                     (Shravani)
│   │   │   ├── treasure_routes.py                  (Shreya)
│   │   │   ├── image_routes.py                     (Shreya)
│   │   │   └── emoji_routes.py                     (Asmita)
│   │   │
│   │   ├── agents/
│   │   │   ├── __init__.py                         (Shreya)
│   │   │   ├── base_agent.py                       (Shreya)
│   │   │   ├── filter_agent.py                     (Shreya)
│   │   │   ├── guard_agent.py                      (Shravani)
│   │   │   ├── treasure_agent.py                   (Shreya)
│   │   │   ├── image_agent.py                      (Shreya)
│   │   │   ├── emoji_agent.py                      (Asmita)
│   │   │   ├── fake_filter_agent.py                (Shreya)
│   │   │   ├── fake_guard_agent.py                 (Shravani)
│   │   │   ├── fake_treasure_agent.py               (Shreya)
│   │   │   ├── fake_image_agent.py                 (Shreya)
│   │   │   └── fake_emoji_agent.py                 (Asmita)
│   │   │
│   │   ├── prompts/
│   │   │   ├── __init__.py                         (Shreya)
│   │   │   ├── filter_prompt.py                    (Shreya)
│   │   │   ├── guard_prompt.py                     (Shravani)
│   │   │   ├── treasure_prompt.py                  (Shreya)
│   │   │   └── emoji_prompt.py                     (Asmita)
│   │   │
│   │   ├── schemas/
│   │   │   ├── __init__.py                         (Shreya)
│   │   │   ├── filter_schema.py                    (Shreya)
│   │   │   ├── guard_schema.py                     (Shravani)
│   │   │   ├── treasure_schema.py                  (Shreya, Shravani)
│   │   │   ├── image_schema.py                     (Shreya)
│   │   │   ├── emoji_schema.py                     (Asmita)
│   │   │   └── agent_health_schema.py              (Shreya)
│   │   │
│   │   ├── services/
│   │   │   ├── gemini_service.py                   (Shreya)
│   │   │   ├── moderation_service.py                (Shreya)
│   │   │   ├── image_generation_service.py          (Shreya)
│   │   │   └── image_storage_service.py             (Shreya)
│   │   │
│   │   ├── integrations/
│   │   │   ├── vertex_ai.py                        (Shreya)
│   │   │   ├── firestore.py                        (Shreya)
│   │   │   ├── cloud_storage.py                    (Shreya)
│   │   │   └── secret_manager.py                   (Shreya)
│   │   │
│   │   └── utils/
│   │       ├── logger.py                           (Shreya)
│   │       ├── image_compression.py                (Shreya)
│   │       ├── signed_url.py                       (Shreya)
│   │       └── retry.py                            (Shreya)
│   │
│   └── tests/
│       ├── __init__.py                             (Shreya)
│       ├── fixtures/
│       │   ├── filter_prompts.json                 (Shreya)
│       │   ├── treasure_examples.json              (Shreya)
│       │   └── image_fixture.jpg                   (Shreya)
│       │
│       ├── test_filter_agent.py                    (Shreya)
│       ├── test_guard_agent.py                     (Shravani)
│       ├── test_treasure_agent.py                  (Shreya)
│       ├── test_image_agent.py                     (Shreya)
│       ├── test_emoji_agent.py                     (Asmita)
│       ├── test_agent_health.py                    (Shreya)
│       └── test_agent_contracts.py                 (Shreya, Shravani, Asmita)
│
├── frontend/
│   ├── README.md                                  (Mrudula, Harsimar)
│   └── prompt_heist_flutter/
│       ├── pubspec.yaml                            (Mrudula)
│       ├── analysis_options.yaml                   (Mrudula)
│       ├── lib/
│       │   ├── main.dart                           (Mrudula)
│       │   ├── app.dart                            (Mrudula)
│       │   ├── routes/
│       │   │   ├── app_router.dart                 (Mrudula)
│       │   │   ├── controller_route.dart           (Harsimar)
│       │   │   ├── audience_route.dart             (Mrudula)
│       │   │   └── player_route.dart               (Mrudula)
│       │   ├── core/
│       │   │   ├── config.dart                     (Mrudula)
│       │   │   ├── api_client.dart                 (Mrudula)
│       │   │   ├── socket_client.dart               (Mrudula)
│       │   │   ├── theme.dart                      (Harsimar)
│       │   │   └── design_widgets.dart             (Harsimar)
│       │   ├── features/
│       │   │   ├── controller/
│       │   │   │   ├── login_screen.dart           (Harsimar)
│       │   │   │   ├── session_screen.dart          (Harsimar)
│       │   │   │   ├── treasure_review_screen.dart  (Harsimar)
│       │   │   │   ├── name_review_screen.dart      (Harsimar)
│       │   │   │   ├── live_monitor_screen.dart     (Harsimar)
│       │   │   │   ├── result_screen.dart           (Harsimar)
│       │   │   │   └── event_day_screen.dart        (Harsimar)
│       │   │   ├── player/
│       │   │   │   ├── booth_code_screen.dart       (Mrudula)
│       │   │   │   ├── join_screen.dart             (Mrudula)
│       │   │   │   ├── lobby_screen.dart            (Mrudula)
│       │   │   │   ├── battle_screen.dart           (Mrudula)
│       │   │   │   ├── prompt_feedback_screen.dart  (Mrudula)
│       │   │   │   └── result_screen.dart           (Mrudula)
│       │   │   └── audience/
│       │   │       ├── idle_screen.dart             (Mrudula)
│       │   │       ├── joining_screen.dart          (Mrudula)
│       │   │       ├── battle_screen.dart           (Mrudula)
│       │   │       ├── result_screen.dart            (Harsimar)
│       │   │       └── emoji_face_widget.dart       (Asmita)
│       │   └── shared/
│       │       ├── countdown_widget.dart             (Mrudula)
│       │       ├── player_slot_widget.dart           (Mrudula)
│       │       └── score_widget.dart                 (Harsimar)
│       └── test/
│           ├── app_router_test.dart                  (Mrudula)
│           └── shared_widgets_test.dart              (Harsimar)
│
├── firebase/
│   ├── firebase.json                               (Shreya)
│   ├── .firebaserc                                 (Shreya)
│   ├── firestore.rules                             (Shravani)
│   ├── firestore.indexes.json                     (Shravani)
│   └── hosting/
│       └── README.md                               (Shreya)
│
├── scripts/
│   ├── run-local.sh                                (Shreya)
│   ├── run-backend.sh                              (Shreya)
│   ├── run-ai-service.sh                           (Shreya)
│   ├── seed-firestore.ts                           (Shravani)
│   ├── event-reset.ts                              (Shreya)
│   ├── filter-fixtures.py                          (Shreya)
│   └── load-test.py                                (Shreya)
│
├── .github/
│   └── workflows/
│       ├── ci.yml                                  (Shreya)
│       ├── deploy-dev.yml                          (Shreya)
│       ├── deploy-prod.yml                         (Shreya)
│       └── firebase-hosting.yml                    (Shreya)
│
└── .vscode/
    ├── extensions.json                             (Shreya)
    ├── launch.json                                 (Shreya)
    └── settings.json                               (Shreya)
