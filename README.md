<div align="center">

# Moonlash Runtime Capability Matrix

An event-driven AI runtime connected to a persistent 3D environment and a 24/7 Discord presence. It coordinates conversation, memory, voice, vision, multiple characters, cameras, lighting, animation, tracking, physics, media, games, and live audience input.

`EVENTS` -> `CONTEXT` -> `SCHEDULING` -> `3D SCENE AND AUDIO` -> `PERSISTENCE`

</div>

## Runtime Flow

<table>
<tr>
<td width="20%"><strong>1. Event normalization</strong><br><sub>Chat, voice, sound, visual media, timers, controls, and audience actions enter a common event model.</sub></td>
<td width="20%"><strong>2. Context enrichment</strong><br><sub>Recent conversation, user memories, persona rules, activity state, vision, and scene state are assembled.</sub></td>
<td width="20%"><strong>3. Priority scheduling</strong><br><sub>Queue order, preparation state, interruption rules, locks, and readiness determine execution.</sub></td>
<td width="20%"><strong>4. Scene execution</strong><br><sub>Speech, character transforms, face, hands, camera, lighting, animation, props, particles, and media are controlled.</sub></td>
<td width="20%"><strong>5. State recording</strong><br><sub>History, datasets, analytics, context backups, pending work, cleanup, and recovery state are written.</sub></td>
</tr>
</table>

## Context, Memory, and Model Control

<table>
<tr>
<td width="33%"><strong>Persistent conversational context</strong><br><sub>Working memory is assembled, trimmed, summarized, searched, backed up, and repaired throughout a session.</sub></td>
<td width="33%"><strong>Priority queue scheduling</strong><br><sub>Routine conversation, ambient behavior, audience events, and staged productions share ordered execution.</sub></td>
<td width="33%"><strong>Background preparation</strong><br><sub>Image generation, vision, model calls, and speech synthesis can begin before an item reaches the front of the queue.</sub></td>
</tr>
<tr>
<td><strong>Selective memory retrieval</strong><br><sub>Personal notes and dated history are searched and inserted into active context when relevant.</sub></td>
<td><strong>Context compaction</strong><br><sub>Old instructions, reactions, duplicate information, and stale events are summarized or removed.</sub></td>
<td><strong>History and dataset logging</strong><br><sub>Readable logs and structured records support recall, analysis, experiments, and later tuning.</sub></td>
</tr>
<tr>
<td><strong>Response validation</strong><br><sub>Empty output, refusals, prompt leakage, repetition, excessive length, and malformed commands are detected.</sub></td>
<td><strong>Recursive response repair</strong><br><sub>Invalid output produces a corrective instruction and another generation attempt before presentation.</sub></td>
<td><strong>Presentation command parsing</strong><br><sub>Speech is separated from face, pose, animation, camera, effect, and voice-tone controls.</sub></td>
</tr>
<tr>
<td><strong>Persona state</strong><br><sub>Behavior rules, relationships, speech patterns, forms, current activity, and scene information remain active across turns.</sub></td>
<td><strong>Context and queue backups</strong><br><sub>Working context and serializable pending work can be restored after ordinary failures or reconnects.</sub></td>
<td><strong>Secondary contexts</strong><br><sub>Additional characters maintain independent persona, memory, behavior, and summarization state.</sub></td>
</tr>
</table>

## Model and Endpoint Evaluation

<table>
<tr>
<td width="33%"><strong>Real-context testing</strong><br><sub>A saved conversational memory slice and realistic prompt are reused across candidates.</sub></td>
<td width="33%"><strong>Broad comparison matrix</strong><br><sub>Many providers, endpoints, model families, model sizes, routing layers, and deployment variants are tested.</sub></td>
<td width="33%"><strong>Direct and production paths</strong><br><sub>Direct requests are compared with the same helper and routing paths used by the live runtime.</sub></td>
</tr>
<tr>
<td><strong>Repeated samples</strong><br><sub>Each selected candidate is called several times with consistent input and generation settings.</sub></td>
<td><strong>Latency measurement</strong><br><sub>Wall-clock response times are recorded, averaged, sorted, and printed for comparison.</sub></td>
<td><strong>Human quality review</strong><br><sub>Persona fidelity, naturalness, verbosity, refusal behavior, control compliance, reliability, and usefulness are inspected.</sub></td>
</tr>
</table>

## Voice Input and Speech Recognition

<table>
<tr>
<td width="33%"><strong>Live microphone acquisition</strong><br><sub>Audio devices are selected, sampled continuously, buffered before speech, and recovered after device failures.</sub></td>
<td width="33%"><strong>Voice-activity detection</strong><br><sub>Multiple detection paths identify speech onset, preserve pre-speech audio, measure silence, and close completed utterances.</sub></td>
<td width="33%"><strong>Streaming speech recognition</strong><br><sub>Partial and committed transcripts support responsive turn handling without waiting for long recordings.</sub></td>
</tr>
<tr>
<td><strong>Turn state</strong><br><sub>Speech start, partial updates, eager endings, resumed turns, finalization, and complete turns are tracked.</sub></td>
<td><strong>Microphone and game audio</strong><br><sub>Human speech and game audio use separate capture, buffering, silence, and transcription behavior.</sub></td>
<td><strong>Noise rejection</strong><br><sub>Quiet clips, short clips, corrupted input, implausible transcripts, and duplicate events are filtered.</sub></td>
</tr>
<tr>
<td><strong>Recorder recovery</strong><br><sub>Repeated read failures trigger recorder recreation without restarting the complete runtime.</sub></td>
<td><strong>Recognition reconnects</strong><br><sub>Lost streaming recognition sessions reconnect and resume audio processing.</sub></td>
<td><strong>Non-speech classification</strong><br><sub>Environmental and game sounds are classified, deduplicated, and inserted into character context.</sub></td>
</tr>
</table>

## Vision and Media Understanding

<table>
<tr>
<td width="33%"><strong>Image analysis</strong><br><sub>Images are downloaded, converted when needed, interpreted, and inserted into conversational context.</sub></td>
<td width="33%"><strong>Fast vision</strong><br><sub>A low-latency visual route returns a useful scene description when response speed matters.</sub></td>
<td width="33%"><strong>Generated-image inspection</strong><br><sub>Generated images are analyzed before Moon reacts, presents them, or publishes them.</sub></td>
</tr>
<tr>
<td><strong>Animated-image vision</strong><br><sub>Representative frames capture motion, visual changes, and the visible result of an animation.</sub></td>
<td><strong>Video vision</strong><br><sub>Short videos are sampled into a manageable frame sequence, interpreted, and removed after processing.</sub></td>
<td><strong>Game vision</strong><br><sub>Gameplay prompts focus analysis on the current game, visible state, action, danger, objective, or unusual event.</sub></td>
</tr>
<tr>
<td><strong>Media URL recovery</strong><br><sub>Expired or failed media links can be refreshed and downloaded through alternate paths.</sub></td>
<td><strong>Vision to context</strong><br><sub>Descriptions are added to the main and secondary character contexts with older visual entries compacted.</sub></td>
<td><strong>Vision to speech</strong><br><sub>Visual analysis can directly produce a queued spoken reaction with synchronized presentation.</sub></td>
</tr>
</table>

## Speech Output and Audio Routing

<table>
<tr>
<td width="33%"><strong>Speech-provider failover</strong><br><sub>Multiple speech services are prioritized and tried in order when generation or streaming fails.</sub></td>
<td width="33%"><strong>Streaming and file synthesis</strong><br><sub>Low-latency streams are used where available. Other paths generate temporary audio files.</sub></td>
<td width="33%"><strong>Speech sanitization</strong><br><sub>Control tags, problematic repetition, unsupported text, and formatting artifacts are removed before synthesis.</sub></td>
</tr>
<tr>
<td><strong>Independent output routing</strong><br><sub>Voice, music, chat, microphone, local output, and community voice output use separate routes.</sub></td>
<td><strong>Playback state</strong><br><sub>Pause, resume, skip, cancel, overlap prevention, active speech tokens, and duration guards control playback.</sub></td>
<td><strong>Audio effects</strong><br><sub>Pitch, echo, reverb, phone filtering, volume, and character-form effects can be applied.</sub></td>
</tr>
<tr>
<td><strong>Independent lip-sync feeds</strong><br><sub>Moon, the streamer, the screen character, and the mascot receive separate mouth-control audio signals.</sub></td>
<td><strong>Temporary-file cleanup</strong><br><sub>Generated speech and converted audio are removed after playback or after a delayed safety window.</sub></td>
<td><strong>Community voice playback</strong><br><sub>Generated audio is converted, retried when necessary, and played into the shared voice channel.</sub></td>
</tr>
</table>

## Complete 3D Environment

<table>
<tr>
<td colspan="3"><strong>Persistent multi-character 3D scene</strong><br><sub>The visual system is a complete environment with a map, multiple characters, several light sources, cameras, props, clothing, particles, collisions, and independently controlled scene objects. It is continuously changed by conversation, performances, controls, and audience interactions.</sub></td>
</tr>
<tr>
<td width="33%"><strong>Environment map</strong><br><sub>Characters occupy a shared navigable set. Scene actions can move them between positions and frame locations as part of a sequence.</sub></td>
<td width="33%"><strong>Independent transforms</strong><br><sub>Each character can be positioned, rotated, shown, hidden, moved, framed, and restored independently.</sub></td>
<td width="33%"><strong>Scene graph control</strong><br><sub>Characters, cameras, lights, props, images, overlays, and effects are controlled as coordinated scene objects.</sub></td>
</tr>
<tr>
<td><strong>Independent animation state</strong><br><sub>Moon, the streamer, screen characters, mascots, and guests receive separate animations, speeds, queues, resets, and idle behavior.</sub></td>
<td><strong>52-channel facial capture</strong><br><sub>High-detail tracking covers brows, eyes, cheeks, jaw, lips, mouth shapes, tongue, and asymmetric expressions.</sub></td>
<td><strong>Expressive hand tracking</strong><br><sub>Wrist orientation, fingers, articulation, and live gestures drive character hands and attached effects.</sub></td>
</tr>
<tr>
<td><strong>Body motion capture</strong><br><sub>Characters can switch between tracked body movement, scripted animation, and fixed scene control.</sub></td>
<td><strong>Multiple light sources</strong><br><sub>Scene lights support performance cues, environment states, and audio-reactive behavior.</sub></td>
<td><strong>Programmatic cameras</strong><br><sub>Direct transforms, presets, smooth movement, relative framing, random views, target orbits, shake, saves, and restoration are supported.</sub></td>
</tr>
<tr>
<td><strong>Wardrobe and meshes</strong><br><sub>Outfits and forms are assembled from controllable clothing and mesh states that persist in character state.</sub></td>
<td><strong>Props</strong><br><sub>Weapons, instruments, food, drinks, phones, and images can be attached, animated, displayed, hidden, and reset.</sub></td>
<td><strong>Particle effects</strong><br><sub>Particles can follow hands, mark attacks, enhance transformations, react to music, or run as timed environment effects.</sub></td>
</tr>
<tr>
<td><strong>Collision and ragdolls</strong><br><sub>Character collision volumes support contact, displacement, physical interactions, and ragdoll response.</sub></td>
<td><strong>Scene state locks</strong><br><sub>Long performances and games prevent conflicting animation, camera, and presentation changes.</sub></td>
<td><strong>Transform inspection</strong><br><sub>Camera position, character transforms, and active animation state can be requested and recovered from runtime output.</sub></td>
</tr>
</table>

## 3D Animation and Scene Command Runtime

<table>
<tr>
<td width="33%"><strong>Expression resolution</strong><br><sub>Exact names, aliases, nearest matches, and model-assisted fallback map requests to available expressions.</sub></td>
<td width="33%"><strong>Animation resolution</strong><br><sub>Groups, exact keys, aliases, nearest matches, and contextual fallback map requests to valid animation assets.</sub></td>
<td width="33%"><strong>Missing-asset telemetry</strong><br><sub>Unknown expressions and animations are recorded and counted to expose gaps between generated commands and scene assets.</sub></td>
</tr>
<tr>
<td><strong>Expression queue</strong><br><sub>Expressions are serialized, deactivated before replacement, timed, and cleared when a neutral face is required.</sub></td>
<td><strong>Animation queue</strong><br><sub>Animations execute in order, apply metadata, hold for a duration, and return to a selected idle state.</sub></td>
<td><strong>Character-specific animation</strong><br><sub>Separate command and reset paths target Moon, the streamer, screen characters, and mascots.</sub></td>
</tr>
<tr>
<td><strong>3D engine recovery</strong><br><sub>Reconnect attempts clear stale queues, cancel old timers, remove listeners, and discard cached transforms.</sub></td>
<td><strong>Payload protection</strong><br><sub>Action length, data size, and buffered socket output are checked before scene commands are sent.</sub></td>
<td><strong>Timed scene restoration</strong><br><sub>Temporary expressions, animations, props, cameras, and effects restore previous or idle state after completion.</sub></td>
</tr>
</table>

## Scene-Side Character and Effects Systems

<table>
<tr>
<td width="33%"><strong>Chat mascot body control</strong><br><sub>The mascot has independent body animation, facial control, lip sync, entrances, effects, and socket commands.</sub></td>
<td width="33%"><strong>First-time chatter welcome</strong><br><sub>The mascot enters, waves, displays the chatter name, and delivers a welcome message.</sub></td>
<td width="33%"><strong>Mascot physical hugs</strong><br><sub>The mascot approaches Moon or the streamer, resolves contact, performs a hug, and returns to normal state.</sub></td>
</tr>
<tr>
<td><strong>Mascot collision</strong><br><sub>Collision volumes allow the mascot to collide physically with other 3D characters.</sub></td>
<td><strong>Mascot socket control</strong><br><sub>Dedicated commands control mascot movement, face, animation, entrances, speech, and reactions.</sub></td>
<td><strong>Legacy mascot support</strong><br><sub>Older mascot behavior and its dedicated ability sequence remain supported.</sub></td>
</tr>
<tr>
<td><strong>Camera programs</strong><br><sub>Quick positions, relative cameras, random views, target orbits, saved states, and cinematic paths are reusable across events.</sub></td>
<td><strong>Automatic collaboration layout</strong><br><sub>A 2D guest can be placed and framed automatically alongside the 3D cast.</sub></td>
<td><strong>Low-cost shadows</strong><br><sub>A custom shadow representation reduces rendering cost while preserving readable character shadows.</sub></td>
</tr>
<tr>
<td><strong>Audio-reactive lighting</strong><br><sub>Selected voice, music, and performance audio sources can drive scene lighting response.</sub></td>
<td><strong>Hand particle trails</strong><br><sub>Tracked hand movement emits particles during gestures, dances, attacks, and performances.</sub></td>
<td><strong>Community streak animations</strong><br><sub>Sustained community activity dispatches scene animations and effects.</sub></td>
</tr>
<tr>
<td><strong>Generated-character reveal</strong><br><sub>Character pulls use image staging, reveal timing, cameras, effects, reaction space, and cleanup.</sub></td>
<td><strong>Horror sequences</strong><br><sub>Scary poses, threatening movement, orbit cameras, weapons, and visual effects produce timed horror presentations.</sub></td>
<td><strong>Cinematic special attacks</strong><br><sub>Music, several camera angles, poses, attack animation, props, effects, and restoration run as one sequence.</sub></td>
</tr>
<tr>
<td><strong>Retaliation system</strong><br><sub>Audience attacks against Moon can select from several counterattacks with independent animations, effects, and timing.</sub></td>
<td><strong>Secondary-character abilities</strong><br><sub>Screen characters can execute character-specific spells with their own animation, effects, audio, and scene commands.</sub></td>
<td><strong>Food deliveries</strong><br><sub>Audience gifts place cookies, cake, pizza, drinks, and snacks into dedicated prop and presentation sequences.</sub></td>
</tr>
</table>

## Screen Characters, Phone Characters, and Mascots

<table>
<tr>
<td width="33%"><strong>Independent screen-character runtime</strong><br><sub>Each screen character loads a persona, scenario, function rules, voice, face data, animation data, and persistent context.</sub></td>
<td width="33%"><strong>Screen-character memory</strong><br><sub>Character context has its own cleanup, memory compaction, rolling summarization, persistence, and duplicate control.</sub></td>
<td width="33%"><strong>Screen-character presentation</strong><br><sub>Speech, lip sync, expression selection, animation selection, function decisions, and scene commands are handled independently.</sub></td>
</tr>
<tr>
<td><strong>Phone characters</strong><br><sub>A caller can reach a selected lore character through a staged, character-specific conversation.</sub></td>
<td><strong>Phone-call lifecycle</strong><br><sub>Caller identity, phone UI, ring or dial audio, caller imagery, subtitles, turns, memory updates, and hang-up restoration are coordinated.</sub></td>
<td><strong>Phone interruption rules</strong><br><sub>Active calls reserve presentation state, reject conflicting calls, and restore prior conversation context afterward.</sub></td>
</tr>
<tr>
<td><strong>Chat mascot persona</strong><br><sub>The mascot has its own voice, movement, expressions, effects, tracking, lip sync, and audience-triggered actions.</sub></td>
<td><strong>Character event sharing</strong><br><sub>Selected chat, voice, game sound, visual, and scene events are propagated to relevant character contexts.</sub></td>
<td><strong>Character persistence</strong><br><sub>Active characters, contexts, visual state, and character flags can survive runtime restarts.</sub></td>
</tr>
</table>

## Interactive Audience Systems

<table>
<tr>
<td width="33%"><strong>Modular discovery</strong><br><sub>Interactive scripts are discovered, normalized into labels, loaded independently, and isolated from unrelated load failures.</sub></td>
<td width="33%"><strong>Preparation phase</strong><br><sub>Image, vision, model, speech, and media work can begin before the visible interaction starts.</sub></td>
<td width="33%"><strong>Execution phase</strong><br><sub>The scheduler grants scene access after preparation and earlier protected work complete.</sub></td>
</tr>
<tr>
<td><strong>Immediate interactions</strong><br><sub>Short sounds, expressions, animations, props, attacks, and reactions can run without lengthy preparation.</sub></td>
<td><strong>Queued productions</strong><br><sub>Long interactions preserve ordering, wait for scene availability, and use presentation locks.</sub></td>
<td><strong>Pending interaction recovery</strong><br><sub>Serializable user, message, label, and prepared state can be restored after a reconnect.</sub></td>
</tr>
<tr>
<td><strong>Targeted physical reactions</strong><br><sub>Audience actions can target Moon, the streamer, a screen character, a guest, the mascot, or the shared scene.</sub></td>
<td><strong>Persistent outfits and forms</strong><br><sub>Form changes update clothing, scene state, model context reminders, and later interaction behavior.</sub></td>
<td><strong>Prompted responses</strong><br><sub>Attention, opinions, ratings, roasts, answers, memories, and highlighted messages enter the conversational scheduler.</sub></td>
</tr>
<tr>
<td><strong>Randomized collection systems</strong><br><sub>Characters, heroes, products, voices, images, and outcomes use staged selection, reveal, reaction, quota, and cleanup behavior.</sub></td>
<td><strong>Generated-media productions</strong><br><sub>Prompts produce images or media that are analyzed, discussed, staged in 3D, published, and removed.</sub></td>
<td><strong>Review and broadcast formats</strong><br><sub>Content can be presented as a review, report, advertisement, phone call, comic, stylized image, or informational segment.</sub></td>
</tr>
<tr>
<td><strong>Audience games</strong><br><sub>Questions, answer boards, semantic guess matching, scores, timers, leaderboards, music, and closing responses form one loop.</sub></td>
<td><strong>Access and rate controls</strong><br><sub>User access, cooldowns, quotas, active-game rules, scene restrictions, and duplicate suppression are enforced.</sub></td>
<td><strong>Multi-surface output</strong><br><sub>Interactions can update the 3D scene, local audio, community audio, chat, overlays, timers, images, and history.</sub></td>
</tr>
</table>

## Full-Song Production

<table>
<tr>
<td colspan="3"><strong>Time-coded music and 3D scene performance</strong><br><sub>A full song runs as a protected production with separate music and vocal channels, a timed cue script, dynamic cameras, character transforms, facial expressions, animation, dance, speed changes, scene commands, and post-song restoration.</sub></td>
</tr>
<tr>
<td width="33%"><strong>Timestamped cues</strong><br><sub>Lyrics, expressions, animations, cameras, character actions, speed, context updates, and scene commands execute at precise offsets.</sub></td>
<td width="33%"><strong>Dynamic camera console</strong><br><sub>Smooth camera moves, character transforms, close views, wide views, and restoration are scripted through the song.</sub></td>
<td width="33%"><strong>Vocal and lip-sync control</strong><br><sub>Music and vocals are routed separately to support independent playback, character mouth movement, and output destinations.</sub></td>
</tr>
<tr>
<td><strong>Animation and dance</strong><br><sub>Timed movement, expression changes, character-specific actions, props, and animation-speed changes follow the performance script.</sub></td>
<td><strong>Lighting and effects</strong><br><sub>Configured scene actions can change lighting, particles, props, camera behavior, and other performance effects.</sub></td>
<td><strong>Protected recovery</strong><br><sub>Ambient behavior stops, camera state is saved, conflicting animation is frozen, and all state is restored after the song.</sub></td>
</tr>
</table>

## Live Platform, Overlays, and Operator Control

<table>
<tr>
<td width="33%"><strong>In-house live-platform client</strong><br><sub>Authentication validation, persistent event sessions, subscription registration, reconnects, and event parsing are implemented in the project.</sub></td>
<td width="33%"><strong>Normalized platform events</strong><br><sub>Chat, follows, raids, cheers, channel-point events, shared-chat filtering, and duplicate suppression use one internal format.</sub></td>
<td width="33%"><strong>Chat batching</strong><br><sub>Single messages can be handled directly while bursts are combined into one context event and response.</sub></td>
</tr>
<tr>
<td><strong>Timed advertising control</strong><br><sub>Ad breaks coordinate countdowns, start and end cues, music, overlays, queue rules, and return behavior.</sub></td>
<td><strong>Keyboard and hardware hotkeys</strong><br><sub>Local controls trigger media, cameras, character actions, scene changes, emergency stops, and runtime functions.</sub></td>
<td><strong>HTTP control endpoints</strong><br><sub>Local hardware and tools invoke stream, queue, media, camera, and 3D scene actions through request-based controls.</sub></td>
</tr>
<tr>
<td><strong>Persistent local command channel</strong><br><sub>Overlays and control surfaces exchange events for scene state, timers, media, status, and operator actions.</sub></td>
<td><strong>Overlay output</strong><br><sub>Large text, subtitles, timers, notifications, song lists, games, leaderboards, images, and status are broadcast to displays.</sub></td>
<td><strong>Intro sequence</strong><br><sub>A dedicated sequence plays the configured introduction video and transitions into normal operation.</sub></td>
</tr>
</table>

## Discord, 24/7 Text, Media, and Voice

<table>
<tr>
<td colspan="3"><strong>Persistent Discord presence</strong><br><sub>Moon remains available in Discord outside stream hours. Discord uses the same core persona, memory, model routing, response validation, vision, image generation, speech, secondary-character, and history systems as the live runtime.</sub></td>
</tr>
<tr>
<td width="33%"><strong>Text channels</strong><br><sub>Selected channels are monitored and routed according to channel, stream state, direct addressing, and recent activity.</sub></td>
<td width="33%"><strong>Direct messages</strong><br><sub>Private messages use a dedicated route while sharing the main identity, memory, and response systems.</sub></td>
<td width="33%"><strong>Mentions and replies</strong><br><sub>Direct mentions, replies to Moon, referenced messages, stickers, and mention targets are resolved before context insertion.</sub></td>
</tr>
<tr>
<td><strong>Channel history</strong><br><sub>Recent messages, channel names, reply chains, and focused history are inserted when a response needs local conversation context.</sub></td>
<td><strong>User identity</strong><br><sub>Aliases and platform identities are resolved so Discord activity maps to the same users and memories used elsewhere.</sub></td>
<td><strong>Reactions and activity</strong><br><sub>Message reactions and community activity can enter context, with older low-value reaction state removed during cleanup.</sub></td>
</tr>
<tr>
<td><strong>Image vision</strong><br><sub>Image attachments are downloaded, converted when needed, analyzed, and inserted into conversational context.</sub></td>
<td><strong>Animated-image vision</strong><br><sub>Animated media is sampled across multiple frames so movement and the visible result are described.</sub></td>
<td><strong>Video vision</strong><br><sub>Video attachments and supported shared-media links are downloaded, sampled into frames, analyzed, and deleted.</sub></td>
</tr>
<tr>
<td><strong>Embed interpretation</strong><br><sub>Video titles, authors, thumbnails, and visual descriptions are extracted from embeds and added to context.</sub></td>
<td><strong>Attachment recovery</strong><br><sub>Expired attachment links can be refreshed before a second download attempt.</sub></td>
<td><strong>Media cleanup</strong><br><sub>Downloaded images, animations, videos, converted files, and generated audio are removed after processing.</sub></td>
</tr>
<tr>
<td><strong>Image generation</strong><br><sub>Discord users can request multiple image formats and character styles through the same generation and visual-analysis pipeline.</sub></td>
<td><strong>Generation controls</strong><br><sub>Prompt checks, length limits, safety handling, cooldowns, per-user quotas, loading messages, and failure output are enforced.</sub></td>
<td><strong>Result publishing</strong><br><sub>Generated images, prompts, descriptions, and fallback media can be posted back to Discord and added to Moon's context.</sub></td>
</tr>
<tr>
<td><strong>Memory commands</strong><br><sub>Users can load person-specific memory, add long-term notes, and search historical conversation.</sub></td>
<td><strong>Character commands</strong><br><sub>Users can list known characters, inspect character prompts, and request character-specific visual formats.</sub></td>
<td><strong>Utility commands</strong><br><sub>Help, songs, time, quota status, drawing modes, comics, and specialized visual requests are available.</sub></td>
</tr>
<tr>
<td colspan="3"><strong>Discord voice conversation</strong><br><sub>Moon can join a voice channel, receive user audio, decode it, detect speaker turns, reject noise, transcribe speech, add it to context, generate a response, and play her voice back into the same channel.</sub></td>
</tr>
<tr>
<td><strong>Speaker-aware capture</strong><br><sub>Per-user speaking events open individual recording streams and preserve speaker identity through transcription.</sub></td>
<td><strong>Turn completion</strong><br><sub>Inactivity closes each utterance. Volume, duration, corruption, and transcript-anomaly checks reject invalid clips.</sub></td>
<td><strong>Voice response scheduling</strong><br><sub>Mentions, speaker identity, queue state, active speech, and character routing determine whether and when Moon responds.</sub></td>
</tr>
<tr>
<td><strong>Voice playback</strong><br><sub>Generated audio is converted to the required channel format, retried after conversion failure, volume-controlled, and cleaned up.</sub></td>
<td><strong>Screen-character routing</strong><br><sub>Mentions can direct a turn to a secondary character with independent context, voice, expression, animation, and lip sync.</sub></td>
<td><strong>Operating modes</strong><br><sub>Channel and response rules adjust for live streaming, Discord-based broadcasting, watch-alongs, and offline operation.</sub></td>
</tr>
</table>

## Reliability and Observability

<table>
<tr>
<td width="33%"><strong>Reconnect and retry handling</strong><br><sub>External services, audio devices, recognition streams, community connections, and the 3D engine have recovery paths.</sub></td>
<td width="33%"><strong>Queue watchdogs</strong><br><sub>Queue processing, scheduling activity, locks, and stalled work are observed during live operation.</sub></td>
<td width="33%"><strong>API analytics</strong><br><sub>Provider, model, purpose, function, timing, and call activity are recorded for production analysis.</sub></td>
</tr>
<tr>
<td><strong>Missing-asset reports</strong><br><sub>Unavailable expressions and animations are counted to guide scene asset and alias updates.</sub></td>
<td><strong>Summary and repetition statistics</strong><br><sub>Context maintenance and repeated response behavior are measured over time.</sub></td>
<td><strong>Temporary-state cleanup</strong><br><sub>Generated files, audio, images, cameras, props, overlays, timers, locks, and scene effects are cleared after use.</sub></td>
</tr>
</table>

## Integrated System Responsibilities

<table>
<tr>
<td width="33%"><strong>Runtime coordination</strong><br><sub>Chat, voice, vision, games, timers, controls, model calls, media preparation, character state, and scene commands share explicit priority, readiness, locking, and interruption rules.</sub></td>
<td width="33%"><strong>Conversational intelligence</strong><br><sub>Persona, long-running context, user memory, retrieval, model routing, validation, repair, summarization, and structured history operate as one conversational subsystem.</sub></td>
<td width="33%"><strong>Multimodal perception</strong><br><sub>Microphones, game audio, environmental sound, images, animated media, videos, and gameplay are converted into normalized context through specialized pipelines.</sub></td>
</tr>
<tr>
<td><strong>3D production environment</strong><br><sub>A persistent map contains independently controlled characters, transforms, detailed tracking, cameras, lights, clothing, props, particles, collision, ragdolls, images, and effects.</sub></td>
<td><strong>Character runtimes</strong><br><sub>The host, streamer, screen characters, phone characters, guests, and mascots use separate combinations of context, voice, lip sync, expression, animation, tracking, memory, and scene control.</sub></td>
<td><strong>Audience interaction runtime</strong><br><sub>Immediate reactions, physical interactions, generated-media productions, randomized collections, phone calls, games, performances, cinematic attacks, limits, persistence, and cleanup share one execution model.</sub></td>
</tr>
<tr>
<td><strong>Media production</strong><br><sub>Speech, music, images, animated media, full-song performances, reports, reviews, overlays, subtitles, timers, leaderboards, and published results are prepared and synchronized.</sub></td>
<td><strong>Discord, operator, and platform control</strong><br><sub>Persistent Discord operation, hotkeys, hardware controls, local sockets, HTTP endpoints, platform events, advertising timers, overlays, and direct scene commands provide operational control.</sub></td>
<td><strong>Reliability and persistence</strong><br><sub>Provider failover, reconnects, recorder recovery, queue backups, context backups, pending work, watchdogs, telemetry, asset reports, and temporary-state cleanup support long-running operation.</sub></td>
</tr>
</table>
