# MacBook Pink Screen and Failed Update Recovery  
**Device:** MacBook Pro (16-inch, 2021)  
**Issue:** Pink screen followed by repeated update failures  
**MDM:** Jamf-managed  

---

## Symptoms  
- Device displayed a **solid pink screen** before crashing.  
- Internal storage nearly full, preventing updates.  
- Multiple update attempts failed.  
- Apple Configurator 2 connection blocked by **MDM administrative lock**.  
- MacBook accessible through **Recovery Mode**.  

---

## Initial Troubleshooting  
1. **Freed disk space** to allow updates.  
2. Attempted standard **macOS update** — failed repeatedly.  
3. Connected to **Apple Configurator 2**, but device remained locked by MDM key.  
   - Retrieved unlock key from internal MDM database.  
   - Configurator stayed locked; no progress possible.  
4. Entered **Recovery Mode** directly from the MacBook.  

---

## Recovery and Reinstallation Steps  
1. In **Recovery Mode**, erased all **APFS volumes**.  
2. Selected **Reinstall macOS** and installed **macOS Sonoma** (latest available version).  
3. System booted successfully but was missing standard Apple apps (e.g., Safari, Mail).  
4. Ran one final **Software Update** to restore full functionality and complete app set.  

---

## Outcome  
- Device fully restored and operational.  
- Standard apps reinstalled after final update.  
- No further crashes or display issues.  
- System ready for reassignment or inventory return.  

---

## Notes  
- MDM lock may persist even when Configurator is connected; direct Recovery reinstall bypasses it.  
- **Low storage** often blocks updates and triggers pink-screen or crash loops.  
- Always run a **final Software Update** after a clean macOS install to restore missing apps and security patches.
