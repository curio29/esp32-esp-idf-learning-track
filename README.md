# esp32-esp-idf-learning-track
ESP32 projects using esp-idf and vscode. 
21-Day Embedded IoT Project Plan (RTOS + MQTT + Mobile
App)
Goal: Complete an industry-grade RTOS-based IoT device project and be interview-ready.
Week 1 — Embedded Foundations + Sensor Bring-up (Days 1–7)
Day 1: Setup + First Flash
Learn: ESP-IDF basics, build/flash/monitor flow.
Do: Install ESP-IDF + VS Code, flash hello_world, capture UART logs screenshot.
Deliverable: GitHub repo created + first commit.
Day 2: GPIO Output (LED Driver)
Learn: GPIO output, pin modes.
Do: Blink LED using ESP-IDF GPIO, create led.c/led.h.
Deliverable: Modular LED driver + logs.
Day 3: GPIO Input (Button + Debounce)
Learn: Pull-up/pull-down, bounce issue.
Do: Read button input, implement software debounce.
Deliverable: Button press toggles LED (stable).
Day 4: UART Logging & Debug Style
Learn: UART + logging levels.
Do: Add structured logs (INFO/ERROR), print system boot info.
Deliverable: Clean log output for debugging.
Day 5: I2C Sensor Integration
Learn: I2C, ACK/NACK, addressing.
Do: Connect I2C sensor (BME280/MPU6050/any), read values and print.
Deliverable: Sensor working with real readings.
Day 6: Timer (Non-blocking periodic read)
Learn: Timers vs delay, periodic scheduling.
Do: Read sensor every 1 second using timer approach, avoid long delays.
Deliverable: Periodic sensor read + stable logs.
Day 7: Code Cleanup + GitHub README v1
Learn: Basic documentation style.
Do: Refactor folder structure, add README (hardware used, how to flash, output logs).
Deliverable: Clean Week-1 milestone on GitHub.
Week 2 — FreeRTOS + Interrupts + Watchdog (Days 8–14)
Day 8: FreeRTOS Tasks (2 tasks)
Learn: Task basics, vTaskDelay.
Do: Create Sensor Task + Logger Task.
Deliverable: Multi-task firmware running.
Day 9: Queue (Sensor → Logger)
Learn: Queue concept.
Do: Send sensor readings via queue, logger prints queue data.
Deliverable: Clean architecture (no global sharing).
Day 10: Mutex/Semaphore (Shared resource)
Learn: Race condition basics.
Do: Add shared I2C resource protection using mutex.
Deliverable: Safe I2C access in multitasking.
Day 11: Interrupt (Button ISR → Task Notify)
Learn: ISR rules, task notification.
Do: Button interrupt triggers control command using task notify (ISR → Control Task).
Deliverable: Interrupt-based event system.
Day 12: PWM Output (Actuator control)
Learn: PWM duty cycle, frequency.
Do: Control LED brightness/motor speed using PWM; map command → PWM.
Deliverable: PWM controlled by task/interrupt.
Day 13: Watchdog Timer + Recovery
Learn: Why WDT exists, system hang cases.
Do: Enable watchdog, simulate hang, ensure system resets safely.
Deliverable: Fault-tolerant firmware.
Day 14: Week-2 Review + Documentation
Learn: Architecture explanation.
Do: Add architecture diagram in README, write tasks & responsibilities, known issues & fixes.
Deliverable: Interview-ready explanation ready.
Week 3 — WiFi + MQTT + Mobile App + Testing (Days 15–21)
Day 15: WiFi Connection (Robust)
Learn: WiFi states, reconnect logic.
Do: Connect WiFi, retry on failure, log IP address.
Deliverable: Stable WiFi connection module.
Day 16: MQTT Publish (JSON Payload)
Learn: MQTT broker/client, topics.
Do: Publish sensor data every 2 sec using JSON (temp, humidity, timestamp).
Deliverable: Data visible on broker.
Day 17: MQTT Subscribe (Remote Control)
Learn: Subscribe callback flow.
Do: Subscribe to control topic, control LED/relay/PWM via MQTT command.
Deliverable: Remote device control works.
Day 18: MQTT + WiFi Reconnect Stability
Learn: Reconnect patterns.
Do: Disconnect WiFi manually, ensure auto reconnect + MQTT re-subscribe.
Deliverable: Production-like reliability.
Day 19: Mobile App (Flutter/Android UI)
Learn: Simple UI principles.
Do: Create app UI: live values, ON/OFF button, status indicator.
Deliverable: App UI ready.
Day 20: App Integration + Real Control
Learn: End-to-end flow.
Do: App sends MQTT command, app displays MQTT sensor data.
Deliverable: Full end-to-end system: Device ↔ Cloud ↔ App.
Day 21: Testing + Final README + Demo Video
Learn: Testing mindset.
Do: Write test cases (sensor fail, wifi drop, mqtt drop, watchdog reset), final README polish, record demo video.
Deliverable: Job-ready GitHub project + proof video.
Daily Output Checklist
Every day you must have at least one output:
3 Code committed
3 Screenshot of logs
3 Short note: What I learned + bug fixed
