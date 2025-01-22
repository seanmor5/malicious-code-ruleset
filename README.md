# malicious-code-ruleset

## Purpose

This repository contains Semgrep rules to detect dynamic code execution and obfuscation, patterns found in nearly 100% of malware-in-code attacks reported to this day. Only rules with low false-positive rates and strong correlation with malicious code are included.

## Supported Languages

Bash  
Clojure  
C#  
Dart  
Go  
Java  
JavaScript  
TypeScript  
Lua  
PHP  
Python  
Ruby  
Rust  
Scala  

## Installation

1. Install [Semgrep](https://semgrep.dev/docs/getting-started):
   ```bash
   pip install semgrep==1.102.0
   ```
2. Clone this repository:
   ```bash
   git clone https://github.com/apiiro/malicious-code-ruleset.git
   ```
3. Run Semgrep with the following command:
   ```bash
   semgrep --config ./malicious-code-ruleset
   ```
   Notice that Semgrep loads the rules corresponding to the extensions of the code files.

## Usage

This ruleset was developed for integration with any CI/CD pipeline, enabling detection at any stage. To monitor pull requests in real-time using this ruleset and trigger policies and workflows, check out Apiiro's [PRevent](https://github.com/apiiro/PRevent.git).

## Contributing

Contributions to improve the ruleset are welcome via pull requests or issues with new patterns (after comprehensive testing) or suggestions.

## License

This repository is licensed under the [MIT License](LICENSE).

---

For more information:  
https://apiiro.com/blog/prevent-malicious-code
