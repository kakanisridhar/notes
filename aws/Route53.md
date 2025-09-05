# Route 53

local dns server 
    -> Root dns server - forwards requests to other servers e.g sees **.com and forwards to The registered top level domain server 
    -> The top level domain server  - Forwards the request to Authoritative servers, e.g sees ***.example.com 
    -> Authoritative servers - maintian records on behalf of clients  