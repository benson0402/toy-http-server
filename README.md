# Toy HTTP Server

A toy HTTP server for learning low-level networking, modern C++ and high-performance design.

## Features

- [ ] HTTP/1.1 Support
- [ ] HTTP/2 Support (via nghttp2)
- [ ] Asynchronous I/O (Boost.Asio)
- [ ] Multi-threaded event-driven architecture
- [ ] TLS (HTTPS) support with OpenSSL
- [ ] Custom routing & static file serving
- [ ] Logging & Metrics API

---

## Tech Stack

| Technology   | Purpose |
|-------------|---------|
| **C++23**   | Modern C++ features |
| **Boost.Asio** | Asynchronous networking |
| **Boost.Beast** | HTTP request handling |
| **CMake** | Build system |
| **vcpkg** | Dependency manager |

<!--
| **OpenSSL** | TLS/HTTPS encryption |
| **nghttp2** | HTTP/2 support |
| **spdlog** | Logging framework |
-->

---

## Roadmap

### Milestone 1: Development Setup & Basic TCP Server
- [x] Install **C++23, Boost, CMake, vcpkg**
- [ ] Create a basic **asynchronous TCP server**

### Milestone 2: Implement HTTP/1.1
- [ ] Read **raw HTTP request data**
- [ ] Parse **HTTP methods, headers, and body**
- [ ] Return a **basic HTTP response**

### Milestone 3: Asynchronous Request Handling
- [ ] Use **Boost.Beast** for HTTP parsing
- [ ] Implement **multi-threaded request handling**

### Milestone 4: Routing & Static File Support
- [ ] Implement a **custom router** (`/api`, `/hello`)
- [ ] Serve **static files** (HTML, CSS, JS)

### Milestone 5: Performance Optimizations
- [ ] Enable **TCP_NODELAY**
- [ ] Use **memory pooling** (`boost::pool`)
- [ ] Benchmark with `wrk`

### Milestone 6: HTTP/2 Support
- [ ] Integrate **nghttp2**
- [ ] Implement **multiplexed requests**

### Milestone 7: TLS & Security Enhancements
- [ ] Add **TLS (HTTPS) support**
- [ ] Enforce **secure headers**

### Milestone 8: Logging & Metrics
- [ ] Implement **structured logging (spdlog)**
- [ ] Expose **/metrics API endpoint**

