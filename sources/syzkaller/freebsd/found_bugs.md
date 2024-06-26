---
status: collected
title: "Found Bugs"
author: Syzkaller Community
collector: jxlpzqc
collected_date: 20240314
link: https://github.com/google/syzkaller/blob/master/docs/freebsd/found_bugs.md
---

# Found Bugs

Newer bugs come first

- [Fix udp_output() lock inconsistency.](https://reviews.freebsd.org/rS346595)
- [Fix IPV6_CHECKSUM computation.](https://reviews.freebsd.org/rS346402)
- [When sending a routing message, don't allow the user to set the RTF_RNH_LOCKED flag in rtm_flags.](https://reviews.freebsd.org/rS346197)
- [Fix an SCTP related locking issue.](https://reviews.freebsd.org/rS346134)
- [Reinitialize multicast source filter structures after invalidation.](https://reviews.freebsd.org/rS346118)
- [Fix a small locking bug in tcp_log_id().](https://reviews.freebsd.org/rS346094)
- [Fix a double free of an SCTP association in an error path.](https://reviews.freebsd.org/rS345525)
- [Reject F_SETLK_REMOTE commands when sysid == 0.](https://reviews.freebsd.org/rS345513)
- [Initialize scheduler specific data for the FCFS scheduler.](https://reviews.freebsd.org/rS345505)
- [Improve locking when tearing down an SCTP association.](https://reviews.freebsd.org/rS345504)
- [Fix more signed unsigned issues in SCTP.](https://reviews.freebsd.org/rS345466)
- [Fix a signed/unsigned bug when receiving SCTP messages.](https://reviews.freebsd.org/rS345465)
- [Limit the size of messages sent on 1-to-many style SCTP sockets with the SCTP_SENDALL flag.](https://reviews.freebsd.org/rS345461)
- [Limit the number of bytes which can be queued for SCTP sockets.](https://reviews.freebsd.org/rS345460)
- [Fix a KASSERT() in tcp_output().](https://reviews.freebsd.org/rS345441)
- [Disallow preemptive creation of wired superpage mappings.](https://reviews.freebsd.org/rS345382)
- [vm_fault_copy_entry: accept invalid source pages.](https://reviews.freebsd.org/rS345324)
- [Fix a bug in the SCTP stream schedulers.](https://reviews.freebsd.org/rS344872)
- [Allocate an association id and register the stcb with holding the lock.](https://reviews.freebsd.org/rS344742)
- [Allow SCTP stream reconfiguration operations only in ESTABLISHED state.](https://reviews.freebsd.org/rS344724)
- [Fix handling of the SCTP_STATUS socket option in early states.](https://reviews.freebsd.org/rS344723)
- [Honor the memory limits provided when processing the SCTP_GET_LOCAL_ADDRESSES socket option.](https://reviews.freebsd.org/rS344708)
- [Check the index hasn't changed after writing the cmp entry.](https://reviews.freebsd.org/rS344517)
- [Improve input validation for raw IPv4 socket using the IP_HDRINCL option.](https://reviews.freebsd.org/rS344048)
- [Fix a locking issue in the IPPROTO_SCTP level SCTP_PEER_ADDR_THLDS socket.](https://reviews.freebsd.org/rS343960)
- [Fix a locking bug in the IPPROTO_SCTP level SCTP_EVENT socket option.](https://reviews.freebsd.org/rS343954)
- [Fix locking for IPPROTO_SCTP level SCTP_DEFAULT_PRINFO socket option.](https://reviews.freebsd.org/rS343951)
- [Fix an off-by-one error in the input validation of the SCTP_RESET_STREAMS socketoption.](https://reviews.freebsd.org/rS343769)
- [Limit the user-controllable amount of memory the kernel allocates via IPPROTO_SCTP level socket options.](https://reviews.freebsd.org/rS343089)
- [Fix getsockopt() for IP_OPTIONS/IP_RETOPTS.](https://reviews.freebsd.org/rS342879)
- [Avoid overfow in vtruncbuf().](https://reviews.freebsd.org/rS342857)
- [Limit option_len for the TCP_CCALGOOPT.](https://reviews.freebsd.org/rS341335)
- [Correct vm_fault_copy_entry() handling of backing file truncation after the file mapping was wired.](https://reviews.freebsd.org/rS338999)
- [In vm_fault_copy_entry(), we should not assert that entry is charged if the dst_object is not of swap type.](https://reviews.freebsd.org/rS338998)
- [Handle a guest executing a vm instruction by trapping and raising an undefined instruction exception.](https://reviews.freebsd.org/rS338957)
- [disallow clock_settime too far in the future to avoid panic.](https://reviews.freebsd.org/rS325825)
- [Fix parsing error when processing cmsg in SCTP send calls.](https://reviews.freebsd.org/rS325046)
