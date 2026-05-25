# PhoenixCastTranscripts

Clean, AI-corrected transcripts of [Phoenix Cast](https://twitter.com/USMC_TFPHOENIX) episodes.

Each episode lives in its own folder (`ep_NNN/`) and contains:

- `phoenix_cast_NNN_..._transcript_corrected.md` — the polished transcript with real speaker names and corrected proper nouns
- - `phoenix_cast_NNN_corrections_changelog.md` — a per-fix audit trail of every change applied vs. the raw Whisper/pyannote output
 
  - Raw transcripts are produced with [Whisper](https://github.com/openai/whisper) (small.en) + [pyannote/speaker-diarization-3.1](https://huggingface.co/pyannote/speaker-diarization-3.1). The cleanup pass is automated via the `phoenix-cast-transcript-cleanup` Claude skill.
  - 
