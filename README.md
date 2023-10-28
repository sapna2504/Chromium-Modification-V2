# Modifications for Static Solution
We have modified the following four files in [chromium](https://github.com/chromium/chromium/) codebase:
- net/http/alternative_service.cc
- net/http/broken_alternative_services.cc
- net/http/http_stream_factory_job_controller.cc
- net/quic/quic_context.h

We have also added the patch file named `modifications.patch`

# Modifications for Dynamic Solution
### Changes in HTTP/2 Connection
We have modified the following files in [chromium](https://github.com/chromium/chromium/) codebase:
- net/http/alternative_service.cc
- net/http/bidirectional_stream_request_info.h
- net/http/broken_alternative_services.cc
- net/http/http_stream_factory.h
- net/http/http_stream_factory.cc
- net/http/network_quality_estimator.cc
- net/http/http_stream_factory_job_controller.cc
- net/spdy/spdy_session.h
- net/spdy/spdy_session.cc
- net/quic/quic_context.h
### Changes in QUIC Connection
- net/third_party/quiche/src/quiche/quic/core/quic_connection_stats.h
- net/third_party/quiche/src/quiche/quic/core/quic_connection.cc
- net/third_party/quiche/src/quiche/quic/core/quic_sent_packet_manager.cc


We have also added the patch file named `5025_quic_dynamic-sol.patch` and `tcp_dynamic_sol.patch`.
`5025_quic_dynamic-sol.patch` contains a patch related to QUIC connection.
`tcp_dynamic_sol.patch` contains patch related to HTTP/2 connection.

We have also added sample files(application logs) for DVL and Rate-Limit UDP.

#Sample Files

### Application and Network logs (chrome/chromium)
1. in-the-wild (only network logs)
2. real-traces (both)
3. original vs modified (both)
4. dynamic-high (both)
5. dynamic-low (both)
6. dynamic-very-low (both)
7. dynamic-solution (both)

Also, we have uploaded the application and network logs of mozilla firefox under dynamic-very-low bandwidth pattern.

### Application and Network logs (geographical locations) 
1. delhi
2. bangalore
3. new-york
4. singapore
5. germany 

# Real World Mahimahi Trace Files
In addition, we have uploaded mahimahi trace files generated from the real pcaps.





