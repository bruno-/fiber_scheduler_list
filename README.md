# Fiber Scheduler List

A list of available Fiber Schedulers for Ruby.

Name | Source | Control passing | Description
--- | --- | --- | ---
`Async::Scheduler` | [link](https://github.com/socketry/async/blob/v2.0.0/lib/async/scheduler.rb) | `Fiber#transfer` | Used with the [async](https://github.com/socketry/async) gem.
`FiberScheduler` | [link](https://github.com/bruno-/fiber_scheduler/blob/3efd4da2e5ad5c639f6d1dfdebc80325a359673f/lib/fiber_scheduler.rb) | `Fiber#transfer` | From [fiber_scheduler](https://github.com/bruno-/fiber_scheduler) gem, aims to be a great default choice.
`IO::Event::Scheduler` | [link](https://github.com/socketry/io-event/blob/b7ce5daa7d036f0db45e1f4e207c6eec10832f2f/examples/scheduler/scheduler.rb) | `Fiber#transfer` | Example Fiber Scheduler from the [io-event](https://github.com/socketry/io-event) gem.
Ruby's test `Scheduler` | [link](https://github.com/ruby/ruby/blob/ruby_3_1/test/fiber/scheduler.rb) | `Fiber.yield` & `Fiber#transfer` | Scheduler from the Ruby repo used for tests.

The best way to get notified when a new Fiber Scheduler is released is to
start watching this repo.

### Related

- [fiber_scheduler_spec](https://github.com/bruno-/fiber_scheduler_spec) provides common tests for Fiber Schedulers and [tests each of them](https://github.com/bruno-/fiber_scheduler_spec/tree/main/spec).
