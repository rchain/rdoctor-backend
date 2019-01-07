## RDoctor backend

RDoctor is a tool for collecting logs mostly from RChain nodes for debugging.
This respository contains the backend part.

To install it:

1. Install nginx, Docker and docker-compose.
2. Clone this repository into e.g. `/srv/rdoctor`.
3. Setup nginx with configuration file in `nginx/`.
4. Run `run` script from the cloned repository.

You can also use it with systemd with bundled `rdoctor.service`:

    systemd link rdoctor.service
    systemd enable rdoctor
    systemd start rdoctor
