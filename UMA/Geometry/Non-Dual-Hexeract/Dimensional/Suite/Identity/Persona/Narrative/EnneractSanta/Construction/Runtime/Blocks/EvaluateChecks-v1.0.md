function EvaluateChecks(check1, check2, tau_ND, kappa, gates):

    // Hard failures override everything
    if check1 == "FAIL" or check2 == "FAIL":
        return "FAIL"

    // Any warning escalates to WARN
    if check1 == "WARN" or check2 == "WARN":
        return "WARN"

    // Otherwise safe
    return "PASS"
