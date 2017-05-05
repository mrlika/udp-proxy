# udpproxy
UDP proxy utility like udpxy implemented with asynchronous I/O (Boost.Asio)

Single threaded application (like Node.js). Can be used as C++ library - everything implemented in single header file (Boost.Asio required).

Options:  
  -h [ --help ]                       Print help message  
  -p [ --port ] arg (=5000)           Port to listen on  
  -a [ --listen ] arg (=0.0.0.0)      Address to listen on  
  -c [ --clients ] arg (=0)           Maximum number of clients to accept (0 = unlimited)  
  -B [ --buffer ] arg (=4096)         Maximum UDP packet data size  
  -R [ --outputq ] arg (=1024)        Maximum output queue length per client (0 = unlimited)  
  -o [ --oqoverflow ] arg (=clearq)   Output queue overflow algorithm: 'clearq' (clear queue) or 'drop' (drop current input data)  
  -v [ --verbose ]                    Enable verbose output  
  -S [ --status ]                     Enable /status URL  
  -M [ --renew ] arg (=0)             renew multicast subscription interval in seconds (0 = disable)  
  -m [ --multicastif ] arg (=0.0.0.0) Multicast interface IP address  
