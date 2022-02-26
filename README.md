# Fiber Scheduler List

A list of available Fiber Schedulers for Ruby.

Name | Ruby | Control passing | Description
--- | --- | --- | ---
[`Async::Scheduler` v1](https://github.com/socketry/async/blob/stable-v1/lib/async/scheduler.rb) | 3.0 | `Fiber.yield` & `Fiber#resume` | Used with the [async](https://github.com/socketry/async) gem v1.
[`Async::Scheduler` v2](https://github.com/socketry/async/blob/v2.0.0/lib/async/scheduler.rb) | 3.1 | `Fiber#transfer` | Used with the [async](https://github.com/socketry/async) gem v2.
[`Evt::Scheduler`](https://github.com/dsh0416/evt) | 3.0 | `Fiber.yield` & `Fiber#resume` | [evt gem](https://github.com/dsh0416/evt).
[`FiberScheduler`](https://github.com/bruno-/fiber_scheduler) | 3.1 | `Fiber#transfer` | Aims to be a great default choice.
[`IO::Event::Scheduler`](https://github.com/socketry/io-event/blob/b7ce5daa7d036f0db45e1f4e207c6eec10832f2f/examples/scheduler/scheduler.rb) | 3.1 | `Fiber#transfer` | Example Fiber Scheduler from the [io-event](https://github.com/socketry/io-event) gem.
[`Libev::Scheduler`](https://github.com/digital-fabric/libev_scheduler) | 3.0 | `Fiber.yield` & `Fiber#resume` | Extracted from [polyphony](https://github.com/digital-fabric/polyphony).
[Ruby's test `Scheduler`](https://github.com/ruby/ruby/blob/ruby_3_1/test/fiber/scheduler.rb) | 3.1 | `Fiber.yield` & `Fiber#resume` | Scheduler from the Ruby repo used for tests.

The best way to get notified when a new Fiber Scheduler is released is to
start watching this repo.


### Related

- Learn more about the Ruby's
  [Fiber Scheduler feature](https://brunosutic.com/blog/ruby-fiber-scheduler).
- [fiber_scheduler_spec](https://github.com/bruno-/fiber_scheduler_spec)
  provides common tests for Fiber Schedulers and
  [tests each of them](https://github.com/bruno-/fiber_scheduler_spec/tree/main/spec).
