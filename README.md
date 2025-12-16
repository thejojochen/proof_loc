# Privacy Preserving Proof of Location
Mock iOS App Attest style location attestations with P256 ECDSA signatures, plus Rust verifier supporting bbox/circle/polygon 

constraint generation: `cargo run -p attestation_mock_client -- gen --lat-deg 37.7749 --lon-deg=-122.4194 --out att.json`

verify: `cargo run -p attestation_verifier -- bbox --attestation att.json --bbox="37.70,-122.52,37.82,-122.35"`
